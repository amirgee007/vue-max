<template>
    <div>
        <button class="btn btn-primary" @click="increment(10)">Increment</button>
        <button class="btn btn-primary" @click="decrement">Decrement</button>
    </div>
</template>

<script>
    export default {
        methods: { 
            increment() {
                this.$store.state.counter+=1;
            },
            decrement() {
                this.$store.state.counter-=1;
            }
        }
    }
</script>