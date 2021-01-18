<template>
  <v-container
    fluid
    class="testimonialWrapper my-16"
  >
      <h3
        class="text-center text-h3 my-8"
      >Hundreds of movers recommend ShyftX </h3>
    <VueSlickCarousel 
    :arrows="false" 
    :dots="false"
    :slidesToShow=1
    :slidesToScroll=1
    :autoplay=true
    >
        <div class="tesitimonialContent d-flex flex-column align-center">
            <h4
                class="text-center text-h5 font-weight-bold my-8"
            >Laura J.</h4>
            <p
                class="text-center"
            >
                Since joining ShyftX, I haven’t had an off day. The platform is really simple to use, and you always know if your bid is the lowest thanks to their simple color coding system.
            </p>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="testimonialImg my-6"
            >
            </v-img>
        </div>
        <div class="tesitimonialContent d-flex flex-column align-center">
            <h4
                class="text-center text-h5 font-weight-bold my-8"
                >Sam L.</h4>
            <p
                class="text-center"
            >
                ShyftX always pays on time – this means that I get to pay my workers and plan my life without having to worry about chasing up payments.
            </p>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="testimonialImg my-6"
            >
            </v-img>
        </div>
        <div class="tesitimonialContent d-flex flex-column align-center">
            <h4
                class="text-center text-h5 font-weight-bold my-8"
            >Robert A.</h4>
            <p
                class="text-center"
            >
                Since signing up with ShyftX, I know that there are no more time wasters. And when I do have an off platform job, I still use their contactless video survey technology to accurately, and safely record the inventory and quote the client.
            </p>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="testimonialImg my-6"
            >
            </v-img>
        </div>
        <div class="tesitimonialContent d-flex flex-column align-center">
            <h4
                class="text-center text-h5 font-weight-bold my-8"
            >Sam L.</h4>
            <p
                class="text-center"
            >
                ShyftX always pays on time – this means that I get to pay my workers and plan my life without having to worry about chasing up payments.
            </p>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="testimonialImg my-6"
            >
            </v-img>
        </div>        
        <div class="tesitimonialContent d-flex flex-column align-center">
            <h4
                class="text-center text-h5 font-weight-bold my-8"
            >Robert A.</h4>
            <p
                class="text-center"
            >
                Since signing up with ShyftX, I know that there are no more time wasters. And when I do have an off platform job, I still use their contactless video survey technology to accurately, and safely record the inventory and quote the client.
            </p>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="testimonialImg my-6"
            >
            </v-img>
        </div>
    </VueSlickCarousel>
    <v-img
        src="/img/testimonialsDots.svg"
        width="150"
        class="testimonialDots"
    ></v-img>
  </v-container>
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  // optional style for arrows & dots
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
    name: "Testimonials",
    components: { 
        VueSlickCarousel 
    },


}
</script>

<style scoped>
.testimonialWrapper {
    background-color: #EEEEEC;
    padding: 80px 0 120px 0;
    position: relative;
    border-radius: 0 0 0 60px;

}
.testimonialWrapper p {
    max-width: 800px;
    font-size: 1.2em;
}
.testimonialDots {
    position: absolute;
    bottom: -48px;
    left: 80px;
    z-index: 1;
}

</style>