<template>
    <v-container
        fluid
        class="my-16 industryPressWrapper"
    >
        <v-container
            class="my-16 industryPressInner"
        >
            <v-row>
                <v-col>
                    <h1
                        class="font-weight-bold text-h3 text-center my-12"
                    >Industry press</h1>
                </v-col>
            </v-row>
            <v-row>
                <v-col
                    cols="6"
                >
                    <v-img
                        src='/img/industryNewsDemo01.jpg'
                        class="blogImg"
                    >
                    </v-img>
                    <h5
                        class="my-6 text-h5 font-weight-bold"
                    >Tech Crunch: Corporate relocation startup Shyft raises $15M</h5>
                </v-col>
                <v-col
                    cols="6"
                >
                    <v-img
                        src='/img/industryNewsDemo02.jpg'
                        class="blogImg"
                    >
                    </v-img>
                    <h5
                        class="my-6 text-h5 font-weight-bold"
                    >Graebel and Shyft Partner to Expand CitySwitcher Digital Marketplace for Lump Sum Transferees</h5>
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
    </v-container>
</template>

<script>
export default {
    name: "BlogList"
}
</script>

<style scoped>
.industryPressInner {
max-width: 1280px;
}
    .blogImg {
    border-radius: 15px;
}
a {
    text-decoration: none;
    color: #fff;
}
h1, h5 {
    color: #fff;
}
.industryPressWrapper {
    background: rgb(150,150,150);
    background: linear-gradient(45deg, rgba(150,150,150,1) 0%, rgba(1,1,1,1) 50%, rgba(183,183,183,1) 100%);
}

</style>