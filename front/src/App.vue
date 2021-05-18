<template>
  <v-app>
    <v-content>
      <Nav/>
    </v-content>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>
import Nav from './components/Nav'


export default {
  name: 'App',
  components: {
    Nav,
  }

};
</script>


<style>
  main {
    background-color : #2c2f33;
    color: white;
  }
</style>
