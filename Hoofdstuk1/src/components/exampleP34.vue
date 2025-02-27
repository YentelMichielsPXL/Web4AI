<template>
    <div class="example">
        <h1>Here is our component:</h1>
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" />
        <p>Your name is:
            <span v-if="name">
                {{ name }}
            </span>
            <span v-else>
                (Not provided)
            </span>
        </p>
    </div>
</template>

<script setup>
import { ref } from 'vue';
const name = ref('');

 
</script>

<style scoped>
 
</style>