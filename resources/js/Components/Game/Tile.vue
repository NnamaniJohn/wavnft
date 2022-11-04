<script setup>
import {computed} from "vue";

const props = defineProps(['index']);

function dragStart(ev, index) {
    ev.dataTransfer.setData("text/plain", index);
}

</script>

<template>
    <a href="#" v-if="index !== 9" :id="'tile' + index" class="w-12 sm:w-18 md:w-24 h-12 sm:h-18 md:h-24 bg-gray-700 flex justify-center items-center transition ease-in-out delay-150 hover:scale-105 focus:scale-105 duration-300 ring-offset-2 border-2 border-gray-800 cursor-pointer text-5xl font-bold text-gray-300 select-none" draggable="true" @dragstart="dragStart($event, index)" @click="$emit('selected')">
        {{ index }}
    </a>
</template>
