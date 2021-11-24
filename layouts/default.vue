<template>
  <v-app>
    <v-hover v-slot="{ hover }" open-delay="15" close-delay="15">
      <v-app-bar :elevation="hover ? 20 : 5" :class="{ 'on-hover':hover }" clipped-left clipped-right app>
        <v-toolbar-title class="mx-16" style="letter-spacing: 1px; font-family: 'Teko', sans-serif;">
          <strong>Alcalde Alejo</strong>
        </v-toolbar-title>
        <v-hover v-slot="{ hover }" open-delay="15" close-delay="15">
          <v-btn :elevation="hover ? 5 : 2" :class="{ 'on-hover':hover }" color="primary" outlined icon style="margin-left:65%;" href="https://www.linkedin.com/in/alejo-alcalde-5a0314215/">
            <v-icon>mdi-linkedin</v-icon>
          </v-btn>
        </v-hover>
        <v-hover v-slot="{ hover }" open-delay="15" close-delay="15">
          <v-btn :elevation="hover ? 5 : 2" :class="{ 'on-hover':hover }" outlined icon href="https://github.com/mayex-gif" style="margin-left: 2%;">
            <v-icon>mdi-github</v-icon>
          </v-btn>
        </v-hover>
        </v-app-bar>
      </v-hover>
    <v-main>
      <Nuxt />
    </v-main>
    <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      title: 'Vuetify.js'
    }
  }
}
</script>
