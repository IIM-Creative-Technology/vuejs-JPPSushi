<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <compteur />
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import compteur from '@/components/compteur.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld, compteur
  }
}
</script>
