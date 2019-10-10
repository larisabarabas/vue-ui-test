<template>
  <div class="myPage">
    <HelloWorld msg="My page here"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'myPage',
  components: {
    HelloWorld
  }
}
</script>
