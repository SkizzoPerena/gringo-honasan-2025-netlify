<template>
    <v-app-bar color="#ce2028" :elevation="3" scroll-behavior="inverted hide" scroll-threshold="800">

        <v-img max-height="45" src="../assets/images/NavIcon.png" @click="scrollHome"/>
        <v-btn variant="text" class="rounded-pill" @click="scrollHome">HOME</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="scrollSino">SINO SI GRINGO?</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="scrollLaws">LAWS & BILLS</v-btn>
        <v-btn variant="text" class="rounded-pill" @click="scrollTest">TESTIMONIES</v-btn>
        <v-spacer></v-spacer>
        <v-btn variant="elevated" color="yellow-accent-4"> JOIN OUR MOVEMENT </v-btn>
        <v-col cols="1"></v-col>
    </v-app-bar>
</template>

<script>


</script>

<style scoped>

</style>
