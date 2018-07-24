<template>
<div>
    <p>Counter is: {{ counter2 }}</p>
    <p>Name is: {{ name }}</p>


</div>
</template>

<script>
    export default {
        props: ['counter2', 'name']
    }
</script>