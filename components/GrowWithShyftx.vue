<template>
  <v-container
    class="my-16"
  >
      <v-row>
          <v-col
            cols=12
          >
            <h1
                class="text-h3 text-center"
            >Grow with ShyftX</h1>
            <p
                class="text-center"
            >Our platform helps brands like these build their thing and keep it growing.</p>
            <VueSlickCarousel 
                :arrows="false" 
                :dots="false"
                :slidesToShow=5
                :slidesToScroll=1
                :autoplay=true
            >
                <a href="https://www.tsishipping.com/"><v-img src=".img/GrowLogo01.png"></v-img></a>
                <a href="https://www.roadwaymoving.com/"><v-img src="/img/GrowLogo02.png"></v-img></a>
                <a href="https://capitolnorthamerican.com/"><v-img src="/img/GrowLogo03.png"></v-img></a>
                <a href="https://movage-moving.com/"><v-img src="/img/GrowLogo04.png"></v-img></a>
                <a href="https://accelerated-international.com/"><v-img src="/img/GrowLogo05.png"></v-img></a>
                <a href="https://www.ekomovers.com/"><v-img src="/img/GrowLogo06.png"></v-img></a>
            </VueSlickCarousel>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  // optional style for arrows & dots
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
    name: "GrowWithShyftx",
    components: { 
        VueSlickCarousel 
    },


}
</script>

<style scoped>
h1.text-h3 {
    font-weight: bold;
}

</style>