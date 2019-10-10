<template>
<div>
    <h2>This is a list</h2>
    <ul>
        <li v-for="product in products">
            {{product.name}}
            <b>{{product.provider}}</b>
        </li>
    </ul>
</div>
</template>

<script>
    export default {
        data() {
            return {
                products: [
                    {id: 1, name: 'iPhone7', provider:"Apple"},
                    {id: 2, name: 'iPhone6', provider:"Apple"}
                ]
            }
        },
    }
</script>

<style scoped>
h2{
    text-align: left;
}
    ul{
        margin:0px;
        padding:0px;    
    }
    li{
        list-style: none;
        text-align: left;
        padding: 5px;
        border: 1px solid lightblue;       
        margin: 10px 0px;
        display: flex;
        justify-content: space-between
    }   

</style>