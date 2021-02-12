<template>
  <section id="port">
    <v-container>
      <h1>Sizga quyidagi xizmatlarni taklif qilamiz</h1>
      <v-row>
        <v-col cols="12" lg="3" md="4" sm="6" v-for="n in item" :key="n.img" >
          <img :src="n.img" alt="" />
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script>
export default {
  data: () => ({
    item: [
      {
        img: require("../assets/1.jpg"),
      },
      {
        img: require("../assets/2.2.jpg"),
      },
      {
        img: require("../assets/3.jpg"),
      },
      {
        img: require("../assets/4.jpg"),
      },
      {
        img: require("../assets/5.jpg"),
      },
      {
        img: require("../assets/6.jpg"),
      },
      {
        img: require("../assets/7.jpg"),
      },
      {
        img: require("../assets/8.jpg"),
      },
    ],
  }),
};
</script>
<style lang="scss" scoped>
section{
  padding:90px 0;
}
h1 {
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 150%;
  text-align: center;
  color: #454545;
  margin-bottom: 60px;
}
img {
  width: 100%;
  height: 100%;
}
</style>