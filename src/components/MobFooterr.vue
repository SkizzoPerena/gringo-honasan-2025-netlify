<template>
    <v-container fluid class=" pa-0 footer-bg gap">
        <v-container>
            <v-container class=" d-flex justify-center pt-7">
                <v-img src="../assets/images/LandingLogo.png" max-width="100"></v-img>
            </v-container>
            <v-container class="pt-0">
                <v-btn block variant="text" rounded color="white"
                    @click="goTo('#mobLanding', { easing: 'easeInOutQuart', duration: 1000, }), drawer = !drawer">Home</v-btn>
                <v-btn block variant="text" rounded color="white"
                    @click="goTo('#mobSino', { easing: 'easeInOutQuart', duration: 1000, }), drawer = !drawer">Sino si
                    Gringo?</v-btn>
                <v-btn block variant="text" rounded color="white"
                    @click="goTo('#mobLawsAndBills', { easing: 'easeInOutQuart', duration: 1000, }), drawer = !drawer">Laws
                    and Bills</v-btn>
                <v-btn block variant="text" rounded color="white"
                    @click="goTo('#mobTestimonies', { easing: 'easeInOutQuart', duration: 1000, }), drawer = !drawer">Testimonies</v-btn>
            </v-container>

            <div class="text-center text-button text-white pb-5">
                CONTACT US<br />
                <v-row justify="center">
                    <v-col cols="auto">
                        <v-btn variant="text" icon="mdi-facebook"></v-btn>
                        <v-btn variant="text" icon="mdi-instagram"></v-btn>
                        <v-btn variant="text" icon="mdi-twitter"></v-btn>
                        <v-btn variant="text" icon="mdi-linkedin"></v-btn>
                    </v-col>
                </v-row>
            </div>

            <v-form v-model="valid">
                <v-text-field density="compact" v-model="email" :rules="emailRules" label="E-mail" bg-color="white"
                    rounded="0"></v-text-field>
                <div class="d-flex justify-center pa-0 ma-0"><v-btn size="large" variant="elevated"
                        color="yellow-accent-4" class=" d-flex justify-center" text="Join our movement"
                        type="submit"></v-btn>
                </div>
            </v-form>

            <div class="text-center text-caption text-white pt-15 ">
                Paid for by the family and friends of Gringo Honasan
                <br />© 2024-2025 Gringo Honasan<br />All Rights Reserved.
            </div>
        </v-container>
    </v-container>
</template>

<script>
import { useGoTo } from 'vuetify'
import AppJoin from './AppJoin.vue';


export default {
    data() {
        return {
            drawer: null,
        }
    },
    setup() {
        const goTo = useGoTo()
        return { goTo }
    },
}
</script>

<style>
.footer-bg {
    background: url('../assets/images/FooterBG.png') no-repeat center center;
    background-size: cover;
}
</style>