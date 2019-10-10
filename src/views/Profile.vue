<template>
    <div>
        <h1>This is Profile page</h1>
        <NewComponent msg="Lalalalala"></NewComponent>
    </div>
</template>

<script>
import NewComponent from '@/components/NewComponent.vue';
export default {
    name:"Profile",
    components:{
        NewComponent
    }
}
</script>