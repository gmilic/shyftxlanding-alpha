<template>
    <v-container
        class="my-16"
    >
        <v-row>
            <v-col>
                <h1
                    class="font-weight-bold text-h3 text-center my-12"
                >Resources to give you the inside track</h1>
            </v-col>
        </v-row>
        <v-row>
            <v-col
                cols="6"
            >
                <v-img
                    src='/img/blogDemo01.jpg'
                    class="blogImg"
                >
                </v-img>
                <h5
                    class="my-6 text-h5 font-weight-bold"
                >Building a high-performance culture in your post-COVID-19 team</h5>
            </v-col>
            <v-col
                cols="6"
            >
                <v-img
                    src='/img/blogDemo02.jpg'
                    class="blogImg"
                >
                </v-img>
                <h5
                    class="my-6 text-h5 font-weight-bold"
                >The Data Is In: Our Industry Report and Pew Research Data Show People Are On The Move</h5>
            </v-col>
        </v-row>
        <v-row>
            <v-col
                class="d-flex justify-end"
            >
                <a href="#">more articles +</a>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: "BlogList"
}
</script>

<style scoped>
.container {
max-width: 1280px;
}
    .blogImg {
    border-radius: 15px;
}
a {
    text-decoration: none;
    color: #333333;
}
</style>