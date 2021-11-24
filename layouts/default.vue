<template>
  <v-app>
    <v-hover v-slot="{ hover }" open-delay="15" close-delay="15">
      <v-app-bar :elevation="hover ? 20 : 5" :class="{ 'on-hover':hover }" clipped-left clipped-right app>
        <v-toolbar-title class="mx-16" style="letter-spacing: 1px; font-family: 'Teko', sans-serif;">
          <strong>Alcalde Alejo</strong>
        </v-toolbar-title>
        <v-btn color="primary" outlined icon @click.stop="clipped = !clipped" style="margin-left:65%;" href="https://www.linkedin.com/in/alejo-alcalde-5a0314215/">
          <v-icon>mdi-linkedin</v-icon>
        </v-btn>
        <v-btn color="" outlined icon @click.stop="clipped = !clipped" href="https://github.com/mayex-gif" style="margin-left: 2%;">
          <v-icon>mdi-github</v-icon>
        </v-btn>
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
