<script setup>
import {Head} from '@inertiajs/inertia-vue3';
import Frame from "@/Components/Game/Frame.vue";
import Board from "@/Components/Game/Board.vue";
import Tile from "@/Components/Game/Tile.vue";
import {computed, onMounted, reactive, ref} from "vue";

const no_of_cols = ref(3)

const tiles = reactive([9, 1, 2, 3, 4, 5, 6, 7, 8])
// const history = reactive([0]);
const selected = ref(0);

function shuffle() {
    let box_to = tiles.indexOf(9);

    let allowed_boxes = allowed_titles(box_to, no_of_cols.value).filter( x => (x >= 1 && x <= 9 && x != null));
    let box_from = allowed_boxes[Math.floor(Math.random() * allowed_boxes.length)];

    move_tile(tiles[box_from], box_to);
}

function move_tile(tile, box_to) {
    const box_from =  tiles.indexOf(tile);
    if (tiles[box_to ] === 9 && allowed_titles(box_to, no_of_cols.value).includes(box_from)) {
        tiles[box_to] = tile;
        tiles[box_from] = 9;
        // history.push(box_to);
    }
}

function shuffle_20() {
    for (let i=0; i <= 200; i++) {
        shuffle();
    }
}

function dragover_handler(ev) {
    ev.preventDefault();
    ev.dataTransfer.dropEffect = "move";
    ev.target.classList.add('border-2')
}

function drop_handler(ev, box_to) {
    ev.preventDefault();
    ev.target.classList.remove('border-2')

    const tile = parseInt(ev.dataTransfer.getData("text/plain"));
    move_tile(tile, box_to);
}

function allowed_titles(index, col) {
    return [index - col, (index % col) === 0 ? null : index - 1, (index % col) === (col - 1) ? null : index + 1, index + col];
}

function select_tile(value) {
    selected.value = value;
}

function move_selected(ev, box_to) {
    ev.preventDefault();
    ev.target.classList.remove('border-2')

    const tile = selected.value;
    move_tile(tile, box_to);
}

const isSorted = computed(() => {
    let second_index;
    for(let first_index = 0; first_index < tiles.length; first_index++){
        second_index = first_index + 1;
        if(tiles[second_index] - tiles[first_index] < 0) return false;
    }
    return true;
})

</script>

<template>
    <Head title="Game" />

    <div class="flex flex-col justify-center items-center w-full h-screen bg-gray-600 select-none">
        <div class="m-5">
            <button @click="shuffle_20" class="py-3 px-12 bg-blue-600 rounded-full text-xl font-bold text-gray-800">Shuffle</button>
        </div>
        <h1 class="text-2xl font-bold m-5 bg-green-600" v-if="isSorted">
            <span class="before:block before:absolute before:-inset-1 before:-skew-y-3 before:bg-green-500 relative inline-block">
                <span class="relative text-white">Congratulation</span>
            </span>
        </h1>
        <Frame>
            <Board :cols="no_of_cols">
                <div class="border-gray-700" :class="value === 0 ? 'hover:border-2' : ''" v-for="(value, index) in tiles" :id="'box_' + index" :key="index" @drop="drop_handler($event, index)" @dragover="dragover_handler" @click="move_selected($event, index)">
                    <Tile :index="value" :key="value" @selected="select_tile(value)" />
                </div>
            </Board>
        </Frame>
    </div>
</template>
