<script setup>
import { computed, ref } from 'vue';
const colorCode = ref('');
</script>

<template>
 <div>
    <label for="color">Color: </label>
    <input type="Text" id="color" v-model="colorCode">
    <p :style="{backgroundColor: colorCode}">Your color is: 
        <span>{{ colorCode }}</span>
    </p>
 </div>
</template>

<style scoped>
 
</style>