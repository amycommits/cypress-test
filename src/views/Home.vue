<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <KitchenSink />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import KitchenSink from '@/components/KitchenSink.vue';

export default {
  name: 'home',
  components: {
    HelloWorld,
    KitchenSink,
  },
};
</script>
