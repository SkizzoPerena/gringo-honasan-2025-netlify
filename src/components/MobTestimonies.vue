<template>
    <v-container fluid class="px-0 bg-grey-lighten-3 gap">
        <v-img src="../assets/images/MobTestHead.png"></v-img>
        <v-container>
            <h2 class="text-center py-2">Ito ang masasabi ng mga nakasama ni Gringo sa kanilang buhay at trabaho</h2>
        </v-container>

        <Carousel v-bind="config">
            <Slide :key="slide">
                <div class="carousel__item"><v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
                        <v-card-item>
                            <v-card-title class="text-subtitle-1">
                                “Mabuhay ka!”
                            </v-card-title>
                        </v-card-item>

                        <v-card-text>
                            <div class="text-caption pb-5">
                                “Isang taong lagi nating maaasahan, laging nakasuporta
                                para sa ating mga kababayan, isang tunay na kaibigan, at
                                talagang Makabayan. Itong taong ito ay parang aming
                                tito-tito sa senado, at talagang sinasaluduhan ko!”
                            </div>

                            <v-row>
                                <v-col cols="5" class="float-start">
                                    <v-img rounded="circle" src="../assets/images/Testimonies/Test Icons-01.jpg" />
                                </v-col>
                                <v-col>
                                    <div class="text-subtitle-2">Ramon "Bong" Revila Jr.</div>
                                    <div class="text-caption">Senator</div>
                                </v-col>
                            </v-row>
                        </v-card-text>

                    </v-card></div>
            </Slide>

            <Slide :key="slide">
                <div class="carousel__item"><v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
                        <v-card-item>
                            <v-card-title class="text-subtitle-1">
                                “Batikang Mambabatas”
                            </v-card-title>
                        </v-card-item>

                        <v-card-text>
                            <div class="text-caption pb-5">
                                “Isa sa mga hindi dapat makalimutan ng publiko ngayong
                                eleksyon (2022), ay si senator Gringo Honasan. Subok na subok
                                na, Kahit sa senado, Kahit bilang secretary ng DICT.
                                Batikang Mambabatas, mahusay, napakabait, at
                                maaasahan.”
                            </div>

                            <v-row>
                                <v-col cols="5" class="float-start">
                                    <v-img max-height="75" rounded="circle"
                                        src="../assets/images/Testimonies/Test Icons-02.jpg" />
                                </v-col>
                                <v-col>
                                    <div class="text-subtitle-2">Sonny Angara</div>
                                    <div class="text-caption">Senator, DepEd Secretary</div>
                                </v-col>
                            </v-row>
                        </v-card-text>

                    </v-card></div>
            </Slide>

            <Slide :key="slide">
                <div class="carousel__item"><v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
                        <v-card-item>
                            <v-card-title class="text-subtitle-1">
                                “Mabuhay ka2!”
                            </v-card-title>
                        </v-card-item>

                        <v-card-text>
                            <div class="text-caption pb-5">
                                “Isang taong lagi nating maaasahan, laging nakasuporta
                                para sa ating mga kababayan, isang tunay na kaibigan, at
                                talagang Makabayan. Itong taong ito ay parang aming
                                tito-tito sa senado, at talagang sinasaluduhan ko!”
                            </div>

                            <v-row>
                                <v-col cols="5" class="float-start">
                                    <v-img max-height="75" rounded="circle"
                                        src="../assets/images/Testimonies/Test Icons-01.jpg" />
                                </v-col>
                                <v-col>
                                    <div class="text-subtitle-2">Ramon "Bong" Revila Jr.</div>
                                    <div class="text-caption">Senator</div>
                                </v-col>
                            </v-row>
                        </v-card-text>

                    </v-card></div>
            </Slide>

            <Slide :key="slide">
                <div class="carousel__item">
                    <v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
                        <v-card-item>
                            <v-card-title class="text-subtitle-1">
                                “Mabuhay ka3!”
                            </v-card-title>
                        </v-card-item>

                        <v-card-text>
                            <div class="text-caption pb-5">
                                “Isang taong lagi nating maaasahan, laging nakasuporta
                                para sa ating mga kababayan, isang tunay na kaibigan, at
                                talagang Makabayan. Itong taong ito ay parang aming
                                tito-tito sa senado, at talagang sinasaluduhan ko!”
                            </div>

                            <v-row>
                                <v-col cols="5" class="float-start">
                                    <v-img max-height="75" rounded="circle"
                                        src="../assets/images/Testimonies/Test Icons-01.jpg" />
                                </v-col>
                                <v-col>
                                    <div class="text-subtitle-2">Ramon "Bong" Revila Jr.</div>
                                    <div class="text-caption">Senator</div>
                                </v-col>
                            </v-row>
                        </v-card-text>
                    </v-card>
                </div>
            </Slide>
        </Carousel>
        <div class="d-flex justify-center">
                <Join />
            </div>
        <div class="gap"></div>
    </v-container>
</template>

<script setup>
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
import { useGoTo } from 'vuetify'

const config = {
    itemsToShow: 1.5,
    wrapAround: true,
    transition: 500,
};

</script>

<style>
.carousel__slide {
    padding: 5;
}

.carousel__viewport {
    perspective: 2000px;
}

.carousel__track {
    transform-style: preserve-3d;
}

.carousel__slide--sliding {
    transition: 0.5s;
}

.carousel__slide {
    opacity: 0.9;
    transform: rotateY(-20deg) scale(0.85);
}

.carousel__slide--active~.carousel__slide {
    transform: rotateY(20deg) scale(0.85);
}

.carousel__slide--prev {
    opacity: 1;
    transform: rotateY(-10deg) scale(0.9);
}

.carousel__slide.carousel__slide--next {
    opacity: 1;
    transform: rotateY(10deg) scale(0.9);
}

.carousel__slide--active {
    opacity: 1;
    transform: rotateY(0) scale(1);
}
</style>