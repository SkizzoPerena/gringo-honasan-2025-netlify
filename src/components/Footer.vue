<template>
    <v-container fluid class=" pa-0 footer-bg" height="70vh">
        <v-container class="fill-height">
            <v-row>
                <v-col cols="7" class="text-center">
                    <v-container max-width="400px" class="fill-height"><div class="text-center align-self-center text-h5 text-white ">
                    <v-img src="../assets/images/LandingLogo.png" class="pb-6"></v-img>
                    Paid for by the family and friends of Gregorio "Gringo" Honasan II
                    <div class="text-body-1"><br/>© 2024-2025 Gringo Honasan<br/>All Rights Reserved.</div>
                </div>
                    
                </v-container>
                </v-col>
                <v-col cols="5" class="text-center">
                    <v-container>
                        <v-card color="#87171b" class="mx-auto my-12 px-2 pb-5 text-center" elevation="10" rounded="0">
                            <v-card-item>
                                <v-card-title class="pt-5 text-h5">
                                    Subscribe to receive updates
                                </v-card-title>
                            </v-card-item>

                            <v-card-text>
                                <div class="text-body-2 pb-5">
                                    Ilagay ang iyong email address upang
                                    maging updated sa mga balita tungkol kay
                                    Gringo Honasan!
                                </div>
                                <v-form v-model="valid">
                <v-text-field v-model="email" :rules="emailRules" label="E-mail" bg-color="white" rounded="0"></v-text-field>

                <v-btn  size="large" variant="elevated" color="yellow-accent-4" class="mt-2" block="true" text="Join our movement" type="submit"></v-btn>
            </v-form>
                            </v-card-text>

                        </v-card>
                    </v-container>
                </v-col>
            </v-row>


        </v-container>
    </v-container>
</template>

<script>
export default {

}
</script>

<style>
.footer-bg {
    background: url('../assets/images/FooterBG.png') no-repeat center center;
    background-size: cover;
}
</style>