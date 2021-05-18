<template>
  <v-app-bar flat>
    <v-app-bar-title>
      <span class="font-weight-light">OneFor</span>
      <span style="color:#2E7D32" class="font-weight-bold">All</span>
    </v-app-bar-title>
    <NavBtn class="ml-lg-14" text="Accueil" redirect="/"/>
    <NavBtn text="Commandes" redirect="/commands"/>
    <NavBtn text="Status" redirect="/status"/>
    <NavBtn text="A propos" redirect="/about"/>
    <v-spacer></v-spacer>
    <v-btn depressed="false" flat color="green darken-3 white--text">
      <v-icon left>mdi-login</v-icon>
      <span>Login</span>
    </v-btn>
    <v-btn depressed="false" class="ml-lg-2" flat color="green darken-3 white--text" href="https://discord.com/api/oauth2/authorize?client_id=780019344511336518&permissions=8&scope=bot" target="_blank">
      <v-icon left>mdi-discord</v-icon>
      <span>Add to discord</span>
    </v-btn>
  </v-app-bar>
</template>

<script>
import NavBtn from "@/components/NavBtn";

export default {
  name: "Nav",
  components: {
    NavBtn,
  }
}
</script>

<style scoped>

</style>