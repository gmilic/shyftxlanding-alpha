<template>
    <v-container
        fluid
        class="my-16 pa-0 appHeroBg"
    >

            <v-row>
                <v-col
                    cols="5"
                    class="pl-14"
                >
                    <h1
                        class="text-h5 my-6"
                    >THE ONLINE MARKETPLACE FOR MOVERS</h1>
                    <h1
                        class="appHeroMainText"
                    >BOOK MOVES
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
export default {
    name: "AppHero"
}
</script>

<style scoped>
.appHeroBg {
    background-image: url('/img/truckWhiteHero.jpg');
    background-repeat: no-repeat;
    background-position: 50vw center;
    background-size: contain;
}

.appHeroMainText {
    font-size: 12vw;
    line-height: .8;
}

</style>