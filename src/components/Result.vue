<template>
<div>
    <p>Counter is: {{ counter }}</p>
    <p>Counter Double: {{ counter2 }}</p>
    <p>Clicks of Numbers: {{ clicks }}</p>


</div>
</template>

<script>
    export default {
        computed: {
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