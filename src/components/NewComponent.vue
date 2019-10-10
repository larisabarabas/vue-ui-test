<template>
    <div class="text-container">
        <h3 v-bind:id="id">{{ msg }}</h3>
        <a v-bind:href="url">Take me to {{ linkName}}</a>
    </div>
</template>

<script>
export default {
    name:"NewComponent",
    props:{
        msg:String,
        id:String,
        url:String,
        linkName:String
    }
}
</script>

<style scoped>
    .text-container{
        padding:20px;
        border: 1px solid goldenrod;
        background-color: antiquewhite;
        margin-top:20px;
    }
</style>