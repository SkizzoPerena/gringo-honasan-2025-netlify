<template>
  <v-app>
    <v-main class="d-none d-lg-block">
      <AppBar />
      <Landing id="landing"/>
      <Sino id="sino"/>
      <Laws id="laws"/>
      <Testimonies id="testimonies"/>
      <Outro/>
      <Footerr />

    </v-main>
    <v-main class="d-lg-none">
      <MobAppBar/>
      <MobLanding id="mobLanding" />
      <MobSino id="mobSino" />
      <MobLaws id="mobLawsAndBills" />
      <MobTestimonies id="mobTestimonies" />
      <MobOutro />
      <MobFooterr />
    </v-main>
  </v-app>
</template>

<script>
export default {

}
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