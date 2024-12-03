<template class="d-lg-block">
    <v-app-bar color="#ce2028" :elevation="3" scroll-behavior="inverted hide" scroll-threshold="800">

        <v-img max-height="45" src="../assets/images/NavIcon.png"  @click="goTo('#landing', { easing: 'easeInOutQuart', duration:1000,})"/>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#landing', { easing: 'easeInOutQuart', duration:1000,})">HOME</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#sino', { easing: 'easeInOutQuart', duration:1000, offset:100,})">SINO SI GRINGO?</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#laws', { easing: 'easeInOutQuart', duration:1000, offset:100,})">LAWS & BILLS</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="goTo('#testimonies', { easing: 'easeInOutQuart', duration:1000, offset:100,})">TESTIMONIES</v-btn>
        <v-spacer></v-spacer>
        <AppJoin/>
        <v-col cols="1"></v-col>
    </v-app-bar>
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

</style>
