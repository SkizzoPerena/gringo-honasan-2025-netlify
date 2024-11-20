<template>
  <v-container fluid class="px-0 bg-grey-lighten-3">
    <div class="divider" />
    <v-col class="px-0" cols="6"><v-img src="../assets/images/TestHead.png"></v-img></v-col>
    <v-container>
      <v-row>
        <v-col cols="7">
          <h1>Ito ang masasabi ng mga nakasama
            ni Gringo sa kanilang buhay at trabaho</h1>
        </v-col>
        <v-col cols="5" align-self="center">
          <v-btn size="large" variant="elevated" color="yellow-accent-4" class="float-end"> JOIN
            OUR MOVEMENT </v-btn>
        </v-col>
      </v-row>

    </v-container>
    <Carousel v-bind="config">
      <Slide :key="slide">
        <div class="carousel__item"><v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
            <v-card-item>
              <v-card-title>
                “Mabuhay ka!”
              </v-card-title>
            </v-card-item>

            <v-card-text>
              <div class="text-body-2 pb-5">
                “Isang taong lagi nating maaasahan, laging nakasuporta
                para sa ating mga kababayan, isang tunay na kaibigan, at
                talagang Makabayan. Itong taong ito ay parang aming
                tito-tito sa senado, at talagang sinasaluduhan ko!”
              </div>

              <v-row>
                <v-col cols="3" class="float-start">
                  <v-img max-height="75" rounded="circle" src="../assets/images/Testimonies/Test Icons-01.jpg" />
                </v-col>
                <v-col>
                  <div class="text-h6">Ramon "Bong" Revila Jr.</div>
                  <div class="text-body-1">Senator</div>
                </v-col>
              </v-row>
            </v-card-text>

          </v-card></div>
      </Slide>

      <Slide :key="slide">
        <div class="carousel__item"><v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
            <v-card-item>
              <v-card-title>
                “Batikang Mambabatas”
              </v-card-title>
            </v-card-item>

            <v-card-text>
              <div class="text-body-2 pb-5">
                “Isa sa mga hindi dapat makalimutan ng publiko ngayong
                eleksyon (2022), ay si senator Gringo Honasan. Subok na subok
                na, Kahit sa senado, Kahit bilang secretary ng DICT.
                Batikang Mambabatas, mahusay, napakabait, at
                maaasahan.”
              </div>

              <v-row>
                <v-col cols="3" class="float-start">
                  <v-img max-height="75" rounded="circle" src="../assets/images/Testimonies/Test Icons-02.jpg" />
                </v-col>
                <v-col>
                  <div class="text-h6">Sonny Angara</div>
                  <div class="text-body-1">Senator, DepEd Secretary</div>
                </v-col>
              </v-row>
            </v-card-text>

          </v-card></div>
      </Slide>

      <Slide :key="slide">
        <div class="carousel__item"><v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
            <v-card-item>
              <v-card-title>
                “Mabuhay ka2!”
              </v-card-title>
            </v-card-item>

            <v-card-text>
              <div class="text-body-2 pb-5">
                “Isang taong lagi nating maaasahan, laging nakasuporta
                para sa ating mga kababayan, isang tunay na kaibigan, at
                talagang Makabayan. Itong taong ito ay parang aming
                tito-tito sa senado, at talagang sinasaluduhan ko!”
              </div>

              <v-row>
                <v-col cols="3" class="float-start">
                  <v-img max-height="75" rounded="circle" src="../assets/images/Testimonies/Test Icons-01.jpg" />
                </v-col>
                <v-col>
                  <div class="text-h6">Ramon "Bong" Revila Jr.</div>
                  <div class="text-body-1">Senator</div>
                </v-col>
              </v-row>
            </v-card-text>

          </v-card></div>
      </Slide>

      <Slide :key="slide">
        <div class="carousel__item">
          <v-card class="mx-auto my-12 px-2 text-left" elevation="10" rounded="0">
            <v-card-item>
              <v-card-title>
                “Mabuhay ka3!”
              </v-card-title>
            </v-card-item>

            <v-card-text>
              <div class="text-body-2 pb-5">
                “Isang taong lagi nating maaasahan, laging nakasuporta
                para sa ating mga kababayan, isang tunay na kaibigan, at
                talagang Makabayan. Itong taong ito ay parang aming
                tito-tito sa senado, at talagang sinasaluduhan ko!”
              </div>

              <v-row>
                <v-col cols="3" class="float-start">
                  <v-img max-height="75" rounded="circle" src="../assets/images/Testimonies/Test Icons-01.jpg" />
                </v-col>
                <v-col>
                  <div class="text-h6">Ramon "Bong" Revila Jr.</div>
                  <div class="text-body-1">Senator</div>
                </v-col>
              </v-row>
            </v-card-text>

          </v-card>
        </div>
      </Slide>

      <template #addons>
        <navigation>
          <template #next>
            <v-btn variant="elevated" color="blue-darken-4" icon="mdi-chevron-right"></v-btn>
          </template>
          <template #prev>
            <v-btn variant="elevated" color="blue-darken-4" icon="mdi-chevron-left"></v-btn>
          </template>
        </navigation>
      </template>
    </Carousel>
    <div class="divider" />
  </v-container>
</template>

<script setup>
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'

const config = {
  itemsToShow: 3.95,
  wrapAround: true,
  transition: 500,
};

</script>

<style>
.carousel__next {
  right: 150px;
  width: 50px;
  height: 50px;
}

.carousel__prev {
  left: 150px;
  width: 50px;
  height: 50px;
}



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