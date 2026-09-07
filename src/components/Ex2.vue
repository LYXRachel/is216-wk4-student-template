<script setup>
    import { ref } from 'vue'

    // Add code here

    // single attribute binding
    const width = ref('200');
    const height = ref('200');
    const image = ref('/assets/me.png');

    // multiple attribute binding
    const size = ref({
        width: '200',
        height: '200',
        src: '/assets/me.png'
    })
</script>

<template>

    <!-- Add code here -->
     <img v-bind:src="image" :width="width" :height="height" />
   
    <img v-bind="size" />
</template>
