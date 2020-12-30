<template>
    <v-container
        fluid
        dark
        class="rowBlackWrraper px-0 my-16"
    >
        <div class="rowBlack">
            <div class="column01">
                <v-img
                    src='/img/BookMoreMoves.svg'
                    class="my-16"
                >
                </v-img>
                <a
                    class="my-8 text-h5"
                >
                    more +
                </a>
            </div>
        </div>
        <div class="column02">
            <v-img
                src='/img/truck-white.png'
                width=100%
            >
            </v-img>
        </div>
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
        min-height: 50vh;
        position: relative;
    }
    a {
        color: #fff;
        display: block;
    }
    .rowBlack {
        border-radius: 0 0 40px 40px;
        width: 100%;
        display: flex;
        position: relative;
        background: linear-gradient(226deg, #000000, #666666);
        background-size: 400% 400%;
        -webkit-animation: blackToGrey 5s ease infinite;
        -moz-animation: blackToGrey 5s ease infinite;
        animation: blackToGrey 5s ease infinite;
        -webkit-clip-path: polygon(0 0, 100% 0, 100% 75%, 40px 100%, 0 100%);
        clip-path: polygon(0 0, 100% 0, 100% 75%, 40px 100%, 0 100%);
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
    .column01 {
        width: 30%;
        margin-left: 100px;
    }
    .column02 {
        width: 70%;
        position: absolute;
        top: 20px;
        right: 0;
    }
</style>