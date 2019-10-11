<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import BaseButton from '@/components/BaseButton.vue'

export default {
  name: 'myPage',
  components: {
    HelloWorld,
    BaseButton
  }
}
</script>

<template>
  <div class="myPage">
    <HelloWorld msg="My page here"/>
    <BaseButton msg="Click here"/>
  </div>
</template>

