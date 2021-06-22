<template>
  <div class="home">
    <HelloWorld msg="Cordelia GUIMS"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Bad+Script&display=swap');
.home{}
font-family:'Bad Script', cursive;
</style>
