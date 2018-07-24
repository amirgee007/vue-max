<template>
<div>
    <p>Counter is: {{ doubleCounter }}</p>
    <p>Counter Double: {{ stringCounter }}</p>
    <p>Clicks of Numbers: {{ clicks }}</p>


</div>
</template>

<script>
    import {mapGetters} from 'vuex';
    export default {
        computed: {
            ...mapGetters([
                'doubleCounter',
                'stringCounter'
            ]),
            counter(){
                return this.$store.state.counter;
            },
            counter2(){
                return this.$store.getters.doubleCounter;
            },
            clicks(){
                return this.$store.getters.stringCounter;
            }
        }
    }
</script>