<script>
export default {
    data() {
        return {
            isShown: false,
        };
    },
    methods: {
        toggle() {
        this.isShown = !this.isShown;
        },
    },
}
</script>

<template>
    <div>
        <button @click="toggle">Click me</button>
        <p 
        id="text" 
        v-show="isShown">
        Lorem ipsum dolor sit amet,...
        </p>
    </div>
</template>


<style scoped>
    button{
        background-color: bisque;
        padding: 10px;
        border:1px solid goldenrod;
        border-radius: 10px;
        border-color: none !important;
        margin-top:10px;
        box-shadow: none !important;    
    }
</style>
