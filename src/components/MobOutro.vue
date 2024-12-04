<template>
  <v-container fluid class="px-0 bg-blue-darken-4 gap">
  <v-container>
    <div class="text-white text-center text-h6 font-weight-bold">Mag-register, at makipagtulungan tungo sa isang baong Pilipinas kasama ang libo-libong Pilipino, sa pangunguna ni Gringo Honasan!
            </div>
            <v-form v-model="valid">
                <v-text-field density="compact" v-model="email" :rules="emailRules" class="pt-6 ma-0" label="E-mail" bg-color="white" rounded="0"></v-text-field>
                <div class="d-flex justify-center pa-0 ma-0"><v-btn  size="large" variant="elevated" color="yellow-accent-4" class="mt-2 d-flex justify-center" text="Join our movement" type="submit"></v-btn>
                </div>
            </v-form>
            <p class="smgap"></p>
        <v-img src="../assets/images/mobtaragvert.png"></v-img>
  </v-container>
  <p class="gap"></p>
  </v-container>
</template>

<script>
export default {

}
</script>

<style>

</style>