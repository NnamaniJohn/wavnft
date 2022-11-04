<script setup>
import { Head } from '@inertiajs/inertia-vue3';

function dragStart(ev) {
    ev.dataTransfer.setData("text/plain", ev.target.id);
}

function dragover_handler(ev) {
    // ev.preventDefault();
    ev.dataTransfer.dropEffect = "move";
    const data = ev.dataTransfer.getData("text/plain");
    console.log(ev.target.clientX);
}
function drop_handler(ev) {
    ev.preventDefault();
    // Get the id of the target and add the moved element to the target's DOM
    const data = ev.dataTransfer.getData("text/plain");
    ev.target.appendChild(document.getElementById(data));
}

</script>

<template>
    <Head title="Drag" />

    <div class="bg-gray-500 w-full h-screen relative" @drop="drop_handler" @dragover="dragover_handler">
        <div id="drag" class="bg-red-400 w-36 h-36 absolute p-8 text-center text-3xl font-bold" draggable="true" @dragstart="dragStart">
            <p>Drag me</p>
        </div>
    </div>
</template>
