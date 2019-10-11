<script>
export default {
    name: 'BaseButton',
    props:{
        msg:String,
    }
}
</script>

<template>
    <button>{{msg}}</button>
</template>

<style scoped>
    button{
        padding: 5px 20px;
        border: 1px solid black;
    }
</style>