<br/>
<template>
    <div>
        <button class="btn btn-primary" @click="asyncIncrement({by: 50, duration:1000})">Another Increment</button>
        <button class="btn btn-primary" @click="decrement">Another Decrement</button>
    </div>
</template>

<script>
    import {mapActions} from 'vuex';
    export default {
        methods: { 
            ...mapActions ([
                'increment',
                'decrement',
                'asyncIncrement'
            ]),

        }
    }
</script>