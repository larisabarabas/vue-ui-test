<template>
    <div>
        <h1>This is Profile page</h1>
        <router-link to="/profile/my-page">MyPage </router-link>
        <NewComponent msg="Lalalalala" id=1 url="https://www.netlify.com" linkName="Netlify"></NewComponent>
        <NewComponent msg="Lalalalala" id=2 url="https://www.google.com" linkName="Google"></NewComponent>
        <ToggleComponent/>  
        <ListComponent/>
    </div>
</template>

<script>
 import NewComponent from '@/components/NewComponent.vue';
 import ToggleComponent from '@/components/ToggleComponent.vue';
 import ListComponent from '@/components/ListComponent.vue';
 
export default {
    name:"Profile",
    components:{
        NewComponent,
        ToggleComponent,
        ListComponent
    }
}
</script>