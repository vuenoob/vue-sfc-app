<script setup>
import {computed, ref} from "vue"
let count = ref(0)
const doubleL = computed(() => 1 + '1')

function increment(){
    count.value++
}
</script>

<template>
    <div>
        He{{ doubleL }}o World!
    </div>
    <button @click="increment()">Clicks {{ count }}</button>
</template>

<style scoped>
div, button{
    padding: 5px;
    margin: v-bind(count + "px")
}
button{
    color: red;
    font-weight: 800;
}
</style>