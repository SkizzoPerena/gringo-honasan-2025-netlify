<template>
  <v-container fluid class=" pa-0 bg" height="120vh">
    <v-toolbar color="transparent" class="text-white">

      <v-img max-height="45" src="../assets/images/NavIcon.png"  @click="goTo('#landing', { easing: 'easeInOutQuart', duration:1000,})"/>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#landing', { easing: 'easeInOutQuart', duration:1000,})">HOME</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#sino', { easing: 'easeInOutQuart', duration:1000, offset:100,})">SINO SI GRINGO?</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#laws', { easing: 'easeInOutQuart', duration:1000, offset:100,})">LAWS & BILLS</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#testimonies', { easing: 'easeInOutQuart', duration:1000, offset:100,})">TESTIMONIES</v-btn>
      <v-spacer></v-spacer>
      <AppJoin/>
      <v-col cols="1"></v-col>
    </v-toolbar>
    <v-container class="fill-height">
      <v-row>
        <v-col cols="6" class="text-center">
          <v-img src="../assets/images/LandingLogo.png"></v-img><br />
          <span class="font-italic text-white">
            <h2 class=" font-weight-light">“ True leadership is not about being in power;</h2>
            <h2 class=" font-weight-light">it's about empowering others.”</h2>
          </span>
          <br />
          <div class="d-flex justify-center">          <Join/>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-container>

</template>

<script>
import { useGoTo } from 'vuetify'
import AppJoin from './AppJoin.vue';

export default {
        setup () {
      const goTo = useGoTo()
      return { goTo }
    },
};
</script>

<style scoped>
.bg {
  background: url('../assets/images/Head BG test2.jpg') no-repeat center center;
  background-size: cover;
}
</style>
