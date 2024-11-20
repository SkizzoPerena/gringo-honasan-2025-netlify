<template ref="Landing">
  <v-container fluid class=" pa-0 bg" height="120vh">
    <v-toolbar color="transparent" class="text-white">

<v-img max-height="45" src="../assets/images/NavIcon.png" @click="scrollSino"/>
<v-btn variant="text" @click="scrollHome">HOME</v-btn>
<v-btn variant="text" @click="scrollSino">SINO SI GRINGO?</v-btn>
<v-btn variant="text" @click="scrollLaws">LAWS & BILLS</v-btn>
<v-btn variant="text" @click="scrollTestimonies">TESTIMONIES</v-btn>
<v-spacer></v-spacer>
<v-btn variant="elevated" color="yellow-darken-1"> JOIN OUR MOVEMENT </v-btn>
<v-col cols="1"></v-col>
    </v-toolbar>
    <v-container class="fill-height">
      <v-row>
        <v-col cols="6" class="text-center">
          <v-img src="../assets/images/LandingLogo.png"></v-img><br/>
          <span class="font-italic text-white">
          <h2 class=" font-weight-light">“ True leadership is not about being in power;</h2>
          <h2 class=" font-weight-light">it's about empowering others.”</h2>
        </span>
          <br/>
          <div class="d-flex justify-center"><v-btn variant="elevated" color="yellow-accent-4" size="large"> JOIN OUR MOVEMENT </v-btn>
        </div>
        </v-col>
    </v-row>
  </v-container>
  </v-container>

</template>

<script setup>
  //
</script>

<style scoped>
.bg {
    background: url( '../assets/images/Head BG test2.jpg') no-repeat center center;
    background-size: cover;}
</style>
