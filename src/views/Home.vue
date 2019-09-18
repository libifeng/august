<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <first/>
   <message/>
   <miss/>
   <action/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import First from '@/components/First.vue'
import Message from '@/components/Message.vue'
import Miss from '@/components/Miss.vue'
import Action from '@/components/Action.vue'
export default {
  name: 'home',
  components: {
    HelloWorld,
    First,
    Message,
    Miss,
    Action
   
  }
}
</script>
