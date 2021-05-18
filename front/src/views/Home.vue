<template>
  <v-container>
    <section>
      <v-flex xs12 sm6 md4 lg3 v-for="feature in features" :key="feature.name">
          <v-card flat class="rounded-lg text-xs-center ma-3"  height="20rem" color="#23272a">
            <v-responsive class="pt-4">
              <v-img :src="feature.img" alt="" height="200px" transition></v-img>
            </v-responsive>
            <v-card-text class="white--text">
              <div class="subheading">{{feature.name}}</div>
              <div class="grey--text">{{feature.description}}</div>
            </v-card-text>
          </v-card>
      </v-flex>


    </section>
  </v-container>
</template>

<script>
import features from '../assets/features'
export default {
  name: 'Home',
  title: 'Acceuil',

  data () {
    return {
      features
    }
  }
}
</script>


