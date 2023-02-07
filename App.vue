<script>
export default {
    data() {
        return {
            count: 0
        }
    },
    computed: {
        doubleL() {
            return 1 + '1';
        }
    },
    methods: {
        increment(){
            this.count++
        }
    }
}
</script>

<template>
    <div>
        He{{ doubleL }}o World!
        <button @click="increment()">Clicks {{ count }}</button>
    </div>
</template>

<style scoped>
div, button{
    padding: 5px;
    margin: 5px
}
button{
    color: red;
    font-weight: 800;
}
</style>