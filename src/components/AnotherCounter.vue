<br/>
<template>
    <div>
        <button class="btn btn-primary" @click="increment">Another Increment</button>
        <button class="btn btn-primary" @click="decrement">Another Decrement</button>
    </div>
</template>

<script>
    import {mapMutations} from 'vuex';
    export default {
        methods: { 
            ...mapMutations ([
                'increment',
                'decrement'
            ])
        }
    }
</script>