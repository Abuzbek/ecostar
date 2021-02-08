<template>
  <v-app>
    <v-app-bar app color="white" height="88px">
      <div style="width:100%;" class="d-flex align-center">
        <img
          alt="star Logo"
          class="shrink mx-8"
          style="flex: 0 0 auto; "
          :src="require('./assets/logo.svg')"
        >
        <v-btn tag="a" v-for="n in buttonLeft" :key="n.name" depressed color="transparent">
          {{ n.name }}
        </v-btn>
      </div>
    </v-app-bar>

    <v-main>
      <Header/>
      <About/>
      <Skill/>
      <Portfolio/>
    </v-main>
  </v-app>
</template>

<script>
import Header from './components/header'
import About from './components/about'
import Skill from './components/section'
import Portfolio from './components/portfolio'


export default {
  name: 'App',

  components: {
    Header,About,Skill,Portfolio
  },

  data: () => ({
    buttonLeft:[
      {
        name:'Biz haqimizda'
      },
      {
        name:'Xizmatlarimiz'
      },
      {
        name:'Kontaktlarimiz'
      },
    ],
  }),
};
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700;800&display=swap');
</style>