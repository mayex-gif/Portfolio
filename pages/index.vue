<template>
  <div>
    <div class="Contenedor" style="margin-top: 2%;">
      <center>
        <img src="mj-ismdf.PNG" style="position: relative; width: 100%; height: 100%;">
      </center>
      <v-divider class="mx-16"></v-divider>
      <v-divider class="mx-16"></v-divider>
      <h3 style="font-family: 'Teko', sans-serif; letter-spacing: 5px ;font-size: 20px; text-align: center; margin: 2%;">PÁGINA INFORMÁTICA - PROYECTO ESCOLAR</h3>
      <center>
        <p>Página realizada como actividad correspondiente a la materia de Marco Jurídico de las actvidades industriales dada en Instituto Superior Manuel de Falla<br>Página informática con respecto al marco jurídico de las actividades industriales - ISMDF Técnico en Programación<br>-<br>La página web fue creada con Vuetify.js framework de Vue.js, framework de nuxt.js, framework de Node.js</p>
        <v-hover v-slot="{ hover }" open-delay="15" close-delay="15">
          <v-btn :elevation="hover ? 10 : 5" :class="{ 'on-hover':hover }" outlined href="https://ismdf-mj.web.app/" style="margin: 2%;">
            <v-text>Ir a la página</v-text>
          </v-btn>
        </v-hover>
      </center>
      <v-divider></v-divider>
      <v-divider class="mb-16"></v-divider>
    </div>
  </div>
</template>
