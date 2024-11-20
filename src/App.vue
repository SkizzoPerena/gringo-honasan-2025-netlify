<template>
  <v-app>
    <v-main>
      <AppBar />
      <Landing />
      <Sino />
      <Laws />
      <Testimonies />
      <Outro />
      <Footer />
    </v-main>

  </v-app>
</template>

<script>
export default {
    methods: {
    scrollHome() {
      this.$refs.Landing?.scrollIntoView({ behavior: 'smooth' });
    },
    scrollSino() {
      this.$refs.Sino?.scrollIntoView({ behavior: 'smooth' });
    },
    scrollLaws() {
      this.$refs.Laws?.scrollIntoView({ behavior: 'smooth' });
    },
    scrollTestimonies() {
      this.$refs.Testimonies?.scrollIntoView({ behavior: 'smooth' });
    },
  },

};
</script>
<style>

.gap {
    padding-top: 50px;
}
.smgap {
    padding-top: 30px;
}
.divider {
    padding-top: 150px;
}
</style>