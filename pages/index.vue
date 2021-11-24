<template>
  <div>
    <div class="Contenedor" style="margin-top: 2%;">
      <h2 style="font-family: 'Teko', sans-serif; position: absolute; letter-spacing: 20px ;font-size: 45px  ; margin-top: 4%; margin-left: 45%;">MARCO JURÍDICO</h2>
      <h3 style="font-family: 'Teko', sans-serif; position: absolute; letter-spacing: 5px ;font-size: 45px  ; margin-top: 33%; margin-left: 32%; text-decoration: underline;">ISMDF</h3>
      <center>
        <img src="https://lh5.googleusercontent.com/hxzUfQ4FR8g8lgbqMddB-JmOEIomXheg6UJADYPGktSC3cRfc2STm2OfO6BSTtFhh3wH_HaKF1BVVRc9R8ZNH9gvuLuUl4vZTQbCBj-3EHK6bAc0hD-Z8ITOOqo8p3XYVZ6NEHs" style="position: relative; width: 98%; height: 580px;">
      </center>
    </div>
    <v-divider class="mx-16"></v-divider>
    <v-divider class="mx-16"></v-divider>
    <v-divider class="mx-16"></v-divider>
    <h3 style="font-family: 'Teko', sans-serif; letter-spacing: 5px ;font-size: 20px; text-align: center; margin: 2%;">PÁGINA INFORMÁTICA - PROYECTO ESCOLAR</h3>
    <center>
      <p>Página realizada como actividad correspondiente a la materia de Marco Jurídico de las actvidades industriales dada en Instituto Superior Manuel de Falla<br>Página informática con respecto al marco jurídico de las actividades industriales - Técnico en Programación</p>
      <v-hover v-slot="{ hover }" open-delay="15" close-delay="15">
        <v-btn :elevation="hover ? 10 : 5" :class="{ 'on-hover':hover }" outlined href="https://ismdf-mj.web.app/" style="margin: 2%;">
          <v-text>Ir a la página</v-text>
        </v-btn>
      </v-hover>
    </center>
    <v-divider class="mx-16"></v-divider>
    <v-divider class="mx-16"></v-divider>
    <v-divider class="mx-16"></v-divider>
  </div>
</template>
