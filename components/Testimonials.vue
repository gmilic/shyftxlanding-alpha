<template>
  <v-container>
    <VueSlickCarousel 
    :arrows="true" 
    :dots="true"
    :slidesToShow=3
    :slidesToScroll=1
    :autoplay=true
    >
        <v-card
            color="#353535"
            dark
            class="pa-4"
            min-height="280"
            max-width="90%"
        >

            <v-card-title 
                class="headline font-weight-bold"
            >
            Laura J.
            </v-card-title>

            <v-card-subtitle
                class="cardSubtitle"
            >
                Since joining ShyftX, I haven’t had an off day. The platform is really simple to use, and you always know if your bid is the lowest thanks to their simple color coding system.
            </v-card-subtitle>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="float-right"
            >
            </v-img>
        </v-card>
        <v-card
            color="#353535"
            dark
            class="pa-4"
            min-height="280"
            max-width="90%"
        >

            <v-card-title 
                class="headline font-weight-bold"
            >
            Sam L.
            </v-card-title>

            <v-card-subtitle
                class="cardSubtitle"
            >
                ShyftX always pays on time – this means that I get to pay my workers and plan my life without having to worry about chasing up payments.
            </v-card-subtitle>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="float-right"
            >
            </v-img>
        </v-card>
        <v-card
            color="#353535"
            dark
            class="pa-4"
            min-height="280"
            max-width="90%"
        >

            <v-card-title 
                class="headline font-weight-bold"
            >
            Robert A.
            </v-card-title>

            <v-card-subtitle
                class="cardSubtitle"
            >
                Since signing up with ShyftX, I know that there are no more time wasters. And when I do have an off platform job, I still use their contactless video survey technology to accurately, and safely record the inventory and quote the client.
            </v-card-subtitle>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="float-right"
            >
            </v-img>
        </v-card>        <v-card
            color="#353535"
            dark
            class="pa-4"
            min-height="280"
            max-width="90%"
        >

            <v-card-title 
                class="headline font-weight-bold"
            >
            Sam L.
            </v-card-title>

            <v-card-subtitle
                class="cardSubtitle"
            >
                ShyftX always pays on time – this means that I get to pay my workers and plan my life without having to worry about chasing up payments.
            </v-card-subtitle>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="float-right"
            >
            </v-img>
        </v-card>        <v-card
            color="#353535"
            dark
            class="pa-4"
            min-height="280"
            max-width="90%"
        >

            <v-card-title 
                class="headline font-weight-bold"
            >
            Robert A.
            </v-card-title>

            <v-card-subtitle
                class="cardSubtitle"
            >
                Since signing up with ShyftX, I know that there are no more time wasters. And when I do have an off platform job, I still use their contactless video survey technology to accurately, and safely record the inventory and quote the client.
            </v-card-subtitle>
            <v-img
                src="/img/fiveStars.svg"
                width="150"
                class="float-right"
            >
            </v-img>
        </v-card>
    </VueSlickCarousel>
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

<style>

</style>