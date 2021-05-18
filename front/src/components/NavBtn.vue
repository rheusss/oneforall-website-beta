<template>
  <v-btn  depressed="false" active-class="green darken-3--text" :to="redirect">
    <span>{{ text }}</span>
  </v-btn>
</template>

<script>
export default {
  name: "NavBtn",
  props: {
    text: String,
    redirect: String
  }
}
</script>


