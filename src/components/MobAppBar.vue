<template>
    <v-app-bar scroll-behavior="inverted hide" scroll-threshold="700" :elevation="2" color="#ce2028" density="compact">
        <template v-slot:prepend>
            <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        </template>
        <v-img src="../assets/images/NavIcon.png" @click="goTo('#mobLanding', { easing: 'easeInOutQuart', duration:1000,})" max-height="35"/>
        <template v-slot:append>
            <v-app-bar-nav-icon disabled color="#ce2028"></v-app-bar-nav-icon>
        </template>

    </v-app-bar>

    
<v-navigation-drawer v-model="drawer" temporary class="bg-blue-darken-4">
        <v-list nav>
            <v-list-item text-color="transparent"></v-list-item>
          <v-list-item title="Home" @click="goTo('#mobLanding', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-list-item title="Sino si Gringo?" @click="goTo('#mobSino', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-list-item title="Laws & Bills" @click="goTo('#mobLawsAndBills', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-list-item title="Testimonies" @click="goTo('#mobTestimonies', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
          <v-divider class="mb-1"></v-divider>
          <v-list-item title="JOIN OUR MOVEMENT" @click="goTo('#mobSino', { easing: 'easeInOutQuart', duration:1000,}), drawer = !drawer"></v-list-item>
        </v-list>

      </v-navigation-drawer>
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

<style></style>