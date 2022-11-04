<script setup>
const props = defineProps(['cols']);
</script>

<template>
    <div :class="`bg-gray-300 grid grid-cols-${cols} gap-1 p-1`">
        <slot />
    </div>
</template>
