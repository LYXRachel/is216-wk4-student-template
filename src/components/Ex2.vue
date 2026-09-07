<script setup>
    import { ref } from 'vue'

    // Add code here

    // single attribute binding
    const width = ref('700');
    const height = ref('400');
    const image = ref('/assets/me.png');

    // multiple attribute binding
    const size = ref({
        width: '700',
        height: '400',
        src: '/assets/me.png'
    })
</script>

<template>

    <!-- Add code here -->
     <img v-bind:src="image" :width="width" :height="height" />
   
    <img v-bind="size" />
</template>
