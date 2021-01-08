<template>
    <v-container
        fluid
        class="my-16 pa-0 appHeroBg"
    >

            <v-row>
                <v-col
                    cols="5"
                    class="pl-14 appHeroMainTextWrapper"
                >
                    <h1
                        class="text-h5 my-6"
                    >THE ONLINE MARKETPLACE FOR MOVERS</h1>
                    <h1
                        class="appHeroMainText appHeroMainText01"
                    >BOOK MOVES
                    </h1>
                    <h1
                        class="appHeroMainText appHeroMainText02"
                    >GET <br />LEADS
                    </h1>
                    <h1
                        class="appHeroMainText appHeroMainText03"
                    >GET PAID <br />FAST
                    </h1>
                    <div
                        class="mainButtonSignUp"
                    >Sign Up For Free
                    </div>
                </v-col>
                <!-- <v-col
                    cols="7"
                >
                    <v-img
                        src="/img/truckWhiteHero.jpg"
                    ></v-img>
                </v-col> -->
            </v-row>
    </v-container>
</template>
<script>
import { gsap } from "gsap";

export default {
    name: "AppHero",
    mounted: function() {
      
      let tl = gsap.timeline({repeat: -1})

      tl
      .from('.appHeroMainText01', {
        rotationX: 90,
        duration: .3,
        ease: "power2.out",
        // delay: .1
      })
      .to('.appHeroMainText01', {
        rotationX: 90,
        duration: .3,
        ease: "power2.out",
        opacity: 0,
        height: 0,
        delay: 3
      })
      .from('.appHeroMainText02', {
        rotationX: 90,
        duration: .3,
        ease: "power2.out",
        // delay: .1
      })
      .to('.appHeroMainText02', {
        rotationX: 90,
        duration: .3,
        ease: "power2.out",
        opacity: 0,
        height: 0,
        delay: 3
      })
      .from('.appHeroMainText03', {
        rotationX: 90,
        duration: .3,
        ease: "power2.out",
        // delay: .1
      })
      .to('.appHeroMainText03', {
        rotationX: 90,
        duration: .3,
        ease: "power2.out",
        opacity: 0,
        height: 0,
        delay: 3
      })

    }
}
</script>

<style scoped>
.appHeroBg {
    background-image: url('/img/truckWhiteHero.jpg');
    background-repeat: no-repeat;
    background-position: 40vw center;
    background-size: contain;
    margin: 128px 0 !important;
}

.appHeroMainText {
    font-size: 12vw;
    font-weight: 400;
    line-height: .8;
    font-family: 'Bebas Neue', 'Roboto', sans-serif;
    position: absolute;
}
.appHeroMainTextWrapper {
    position: relative;
    height: 30vw;
}
.mainButtonSignUp {
    position: relative;
    top: 20vw;
}
</style>