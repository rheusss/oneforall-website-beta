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

export default {
  name: 'Home',
  title: 'Acceuil',

  data () {
    return {
      features : [
        {name: "Un puissant antiraid", img: "https://cdn.discordapp.com/attachments/820031925389230110/844176365845479434/dekuPunch.gif", description:"description"},
        {name : "Une automodération" , img: "https://thumbs.gfycat.com/AlarmingTatteredKiwi-max-1mb.gif", description:"description"},
        {name : "Des outils pour faciliter la gestion de votre serveur", img:"https://i.pinimg.com/originals/b8/24/77/b824773317a65cc50c85d942f88c8fe3.gif", description: "description"}
      ]
    }
  }
}
</script>


