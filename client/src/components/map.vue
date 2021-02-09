<template>
  <div class="map">
    <v-container class="py-none">
      <v-row>
        <v-col cols="12" lg="5" md="6" sm="8" class="contact">
          <contact />
        </v-col>
      </v-row>
    </v-container>
    <iframe class="iframe" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d23973.30527343497!2d69.24014154717683!3d41.31619086448038!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38ae8b40d847941d%3A0x5765a18b352df71e!2sTashkent%20City%20Park!5e0!3m2!1suz!2s!4v1612853641073!5m2!1suz!2s" width="100%" height="450" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
    <iframe class="iframe_sm" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d23973.30527343497!2d69.24014154717683!3d41.31619086448038!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38ae8b40d847941d%3A0x5765a18b352df71e!2sTashkent%20City%20Park!5e0!3m2!1suz!2s!4v1612853641073!5m2!1suz!2s" width="100%" height="450" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
  </div>
</template>
<script>
import contact from "./contact";
export default {
  components: {
    contact,
  },
};
</script>
<style lang="scss" scoped>
.map{
  position: relative;
  .iframe{
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    width: 100%;
    z-index: 1;
  }
  .contact{
    position: relative;
    z-index: 3;
     padding-bottom: 0px !important;
  }
  .py-none{
    padding-bottom: 0px !important;
  }
  .iframe_sm{
    display: none;
  }
  @media (max-width:599px) {
    .iframe{
      display: none;
    }
    .iframe_sm{
      display: block;
    }
  }
}
</style>
