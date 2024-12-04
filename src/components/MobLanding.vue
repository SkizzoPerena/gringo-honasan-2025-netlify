<template>
    <v-container fluid class="pa-0 mobbg" height="100vh">
        <v-toolbar color="transparent" density="compact">
        <template v-slot:prepend>
            <v-app-bar-nav-icon @click.stop="drawer = !drawer" color="white"></v-app-bar-nav-icon>
        </template>


    </v-toolbar>

    
<v-navigation-drawer v-model="drawer" temporary class="bg-blue-darken-4">
        <v-list nav>
          <v-list-item title="Home" @click="goTo('#mobLanding', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-list-item title="Sino si Gringo?" @click="goTo('#mobSino', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-list-item title="Laws & Bills" @click="goTo('#mobLawsAndBills', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-list-item title="Testimonies" @click="goTo('#mobTestimonies', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-divider class="mb-1"></v-divider>
          <v-list-item title="JOIN OUR MOVEMENT" @click="goTo('#mobLanding', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
        </v-list>

      </v-navigation-drawer>
        <v-container height="10vh"></v-container>
        <v-img src="../assets/images/MobLanding.png" />

        <v-container class="text-center"><span class="font-italic text-white">
                <h4 class=" font-weight-light">“ True leadership is not about being in power;</h4>
                <h4 class=" font-weight-light">it's about empowering others.”</h4>
            </span>
            <br />

            <div class="d-flex justify-center">
                <Join />
            </div>
        </v-container>

    </v-container>
</template>

<script>
import { useGoTo } from 'vuetify'
import AppJoin from './AppJoin.vue';


export default {
    data () {
      return {
        drawer: null,
      }
    },
    setup () {
      const goTo = useGoTo()
      return { goTo }
    },
}
</script>

<style>
.mobbg {
    background: url('../assets/images/Head BG.png') no-repeat center center;
    background-size: cover;
}
</style>