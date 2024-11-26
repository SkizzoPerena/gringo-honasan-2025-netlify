<template>
    <v-dialog max-width="500">
        <template v-slot:activator="{ props: activatorProps }">
            <v-btn v-bind="activatorProps" variant="elevated" color="yellow-accent-4"
                text="Join our movement"></v-btn>
        </template>

        <template v-slot:default="{ isActive }">
            <v-card color="#ce1126" class="mx-auto my-12 px-2 pb-5 text-center" elevation="10" rounded="0">
                <div d-flex class="pa-0 ma-0 pt-2"><v-btn size="x-small" icon="mdi-close" variant="text" class="float-end" @click="isActive.value = false"></v-btn></div>
                <v-card-item class=" pt-0 mt-0">

                    <v-card-title class="text-h5">
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
                        <v-text-field v-model="email" :rules="emailRules" label="E-mail" bg-color="white"
                            rounded="0"></v-text-field>

                        <v-btn size="large" variant="elevated" color="yellow-accent-4" class="mt-2" block="true"
                            text="Join our movement" @click="goTo(0, { container: '#laaand' })"></v-btn>
                    </v-form>
                </v-card-text>

            </v-card>

        </template>
    </v-dialog>
</template>

<script>
export default {

}
</script>

<style>

</style>