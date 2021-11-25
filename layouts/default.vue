<template>
  <v-app>
    <v-hover v-slot="{ hover }" open-delay="15" close-delay="15">
      <v-app-bar :elevation="hover ? 20 : 5" :class="{ 'on-hover':hover }" clipped-left clipped-right app>
        <v-toolbar-title class="ml-0" style="letter-spacing: 1px; font-family: 'Teko', sans-serif; text-align: center;">
          <strong>Alcalde Alejo Emanuel</strong>
        </v-toolbar-title>
      </v-app-bar>
      </v-hover>
    <v-main>
      <Nuxt />
    </v-main>
  <v-footer color="primary lighten-1 ma-0" padless>
    <v-col justify="center" no-gutters>
      <v-col class="py-4 text-center">
        <v-row class="flex-column">
          <strong style="font-family: 'Teko', sans-serif; letter-spacing: 5px;" class="mt-5">CONTACTO</strong>
          <v-btn outlined v-for="(item, i) in botones" :key="i" :href="item.to" text rounded class="my-2" style="width: 84%; margin-left: 8%; background: #fff;">
            <v-icon :color="item.color">{{ item.icon }}</v-icon>
            <p class="ma-2">{{ item.text }}</p>
          </v-btn>
        </v-row>
      </v-col>
        <v-divider class="pb-1 mt-2"></v-divider>
        <v-card-text class=" text-center white--text">
          Full responsive website
        </v-card-text>
        <v-divider class="my-2"></v-divider>
        <v-card-text class="py-1  text-center white--text">
          <v-icon color="white">mdi-copyright</v-icon>
          Copyright {{ new Date().getFullYear() }} — Alcalde Alejo Emanuel— <strong>Vuetify</strong>
        </v-card-text>
    </v-col>
  </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      title: 'Vuetify.js',
      botones: [
        {
          icon: 'mdi-instagram',
          color: '#d6249f',
          to: 'https://www.instagram.com/alca.alejo/',
          text: 'alca.alejo',
        },
        {
          icon: 'mdi-twitter',
          color: '#00acee',
          to: 'https://www.twitter.com/alca_alejo/',
          text: 'alca_alejo',
        },
        {
          icon: 'mdi-whatsapp',
          color: '#00bb2d',
          to: 'https://wa.me/543516845448',
          text: '+54 0351 684 5448',
        },
        {
          icon: 'mdi-gmail',
          color: '#BB001B',
          to: 'mailto:alcaldealejo53@gmail.com',
          text: 'alcaldealejo53@gmail.com',
        },
        {
          icon: 'mdi-github',
          color: '',
          to: 'https://github.com/mayex-gif',
          text: 'mayex-gif',
        },
        {
          icon: 'mdi-linkedin',
          color: '#0e76a8',
          to: 'https://www.linkedin.com/in/alejo-alcalde-5a0314215/',
          text: 'Alejo Alcalde',
        },  
      ],
    }
  }
}
</script>
