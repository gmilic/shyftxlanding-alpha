<template>
    <v-container
        class="py-16 bg-x"
    >
        <v-row>
            <v-col
                class="text-center"
            >
                <h1
                    class="text-h3 my-8 font-weight-bold"
                >Start your business journey with Shyft</h1>
                <h4
                    class="text-h6 my-8"
                >We help you get instant access to highly qualified moves and to finally say goodbye to off-seasons, whilst bringing great solutions like our contactless video surveying tool.</h4>
                <v-btn
                    elevation="2"
                    outlined
                    dark
                >REQUEST DEMO</v-btn>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: "StartBusinessJourney"
}
</script>

<style scoped>
    h4 {
        max-width: 600px;
        margin: 0 auto;
    }
    .bg-x {
        background: url('/img/bg-x.png');
        background-repeat: no-repeat;
        background-position: center right;
        background-size: contain;
    }
    .container {
    max-width: 960px;
    }
</style>