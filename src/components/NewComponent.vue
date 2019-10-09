<template>
    <div class="text-container">
        <h3>{{ msg }}</h3>
    </div>
</template>

<script>
export default {
    name:"NewComponent",
    props:{
        msg:String
    }
}
</script>

<style scoped>
    .text-container{
        padding:20px;
        border: 1px solid goldenrod;
        background-color: antiquewhite
    }
</style>