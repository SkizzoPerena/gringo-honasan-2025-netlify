<template>
    <v-container fluid class="px-0 bg-blue-darken-4">
        <div class="divider" id="outro" />
        <v-container>
            <div class="text-white text-center text-h3 font-weight-bold">Mag-register, at makipagtulungan tungo sa isang
                <div class="h3-spacing" />baong Pilipinas kasama ang libo-libong Pilipino,
                <div class="h3-spacing" /> sa pangunguna ni Gringo Honasan!
            </div>
            <v-row  justify="center" class="gap">

            <v-col cols="8">
            <v-form v-model="valid" class="d-flex">
                <v-text-field v-model="email" :rules="emailRules" label="E-mail" class="pr-10" bg-color="white" rounded="0"></v-text-field>

                <v-btn  size="large" variant="elevated" color="yellow-accent-4" class="mt-2" text="Join our movement" type="submit"></v-btn>
            </v-form>
        </v-col>


        </v-row>
        <p class="gap"></p>
        <v-img src="../assets/images/TaraG.png"></v-img>
        </v-container>
        <div class="gap" />
    </v-container>
</template>

<script>
export default {

}
</script>

<style>
.h3-spacing {
    padding-top: 20px;
}
</style>