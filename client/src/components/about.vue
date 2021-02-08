<template>
  <section class="about">
    <v-container>
      <h1 style="margin-bottom:80px;" class="text-center">EcoStar bu</h1>
      <v-row>
        <v-col cols="12" lg="4" class="d-flex justify-center align-center flex-column">
          <img class="mb-8" src="../assets/icon1.svg" alt="">
          <h3>Hamyonbop narxlar</h3>
        </v-col>
        <v-col cols="12" lg="4" class="d-flex justify-center align-center flex-column">
          <img class="mb-8" src="../assets/icon2.svg" alt="">
          <h3>Yuqori sifat</h3>
        </v-col>
        <v-col cols="12" lg="4" class="d-flex justify-center align-center flex-column">
          <img class="mb-8" src="../assets/icon3.svg" alt="">
          <h3>Unikal dizayn</h3>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script>
export default {
  
}
</script>
<style lang="scss" scoped>
section.about{
  padding-bottom: 120px;
  padding-top: 60px;
  background: url('../assets/aboutbg.jpg') no-repeat center center / cover;
}
</style>