<template>
    <v-container
        fluid
        dark
        class="rowBlackWrraper px-0 my-16"
    >
        <div class="rowBlack">
        </div>
            <v-row
                class="mainContent"
            >
                <v-spacer></v-spacer>
                <v-col
                    cols="3"
                >
                    <v-img
                        src='/img/BookMoreMoves.svg'
                        class="my-8"
                    >
                    </v-img>
                    <a

                    >
                        more +
                    </a>
                </v-col>
                <v-col
                    cols="8"
                    class="whiteTruck"
                >
                    <v-img
                        src='/img/truck-white.png'
                        width=100%
                    >
                    </v-img>
                </v-col>
            </v-row>
    </v-container>
</template>

<script>
export default {
    name: "BookMoreMovesTruck"
}
</script>

<style scoped>
    h1 {
        color: #fff;
    }
    .whiteTruck {
        overflow: hidden;
    }
    .rowBlackWrraper {
        position: relative;
    }
    .mainContent {
        position: relative;
        z-index: 9;
    }
    a {
        color: #fff;
    }
    .rowBlack {
    border-radius: 0 0 40px 40px;
    height: 300px;
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background: linear-gradient(226deg, #000000, #494949);
    background-size: 400% 400%;
    -webkit-animation: blackToGrey 49s ease infinite;
    -moz-animation: blackToGrey 49s ease infinite;
    animation: blackToGrey 49s ease infinite;
}

    @-webkit-keyframes blackToGrey {
        0%{background-position:99% 0%}
        50%{background-position:2% 100%}
        100%{background-position:99% 0%}
    }
    @-moz-keyframes blackToGrey {
        0%{background-position:99% 0%}
        50%{background-position:2% 100%}
        100%{background-position:99% 0%}
    }
    @keyframes blackToGrey {
        0%{background-position:99% 0%}
        50%{background-position:2% 100%}
        100%{background-position:99% 0%}
    }
</style>