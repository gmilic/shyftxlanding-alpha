<template>
  <v-container
    fluid
    class="secondRowWrapper py-16"
  >
    <v-container>
        <v-row>
            <v-col
                cols=12
                md=6
            >
                <v-row
                    class="firstRow"
                >
                    <v-col
                        cols=12
                        md=5
                        class="d-flex justify-md-end align-start"
                    >
                        <img
                            src="/img/secondRowIcon01.svg"
                            class="secondRowIcon"
                            
                            width="130"
                        />
                    </v-col>
                    <v-col
                        cols=12
                        md=7
                    >
                        <h1
                            class="text-h4"
                        >Pre vetted corporate leads
                        </h1>
                        <h2
                            class="text-h6"
                        >
                        Access thousands of qualified leads with survey and inventory already completed - all you have to do is place your bid and secure business year round. 
                        </h2>
                    </v-col>
                </v-row>
            </v-col>
            <v-col
                cols=12
                md=6
            >
                <v-row>
                    <v-col
                        cols=12
                        md=5
                        class="d-flex justify-md-end align-start"
                    >
                        <img
                            src="/img/secondRowIcon02.svg"
                            class="secondRowIcon"
                            
                            width="120"
                        />
                    </v-col>
                    <v-col
                        cols=12
                        md=7
                    >
                        <h1
                            class="text-h4"
                        >Get paid twice as fast
                        </h1>
                        <h2
                            class="text-h6"
                        >
                        Our Net D is twice as fast as industry average - we partner with lump sum corporate clients, which enables us to pay out faster. 
                        </h2>
                    </v-col>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {

}
</script>

<style scoped>
.secondRowWrapper {
    background: linear-gradient(29.9deg, rgba(254, 254, 254, 0.96) -84.55%, #292929 52.83%);
    border-radius: 0 0 48px 48px;
    -webkit-clip-path: polygon(0 0, 100% 0, 100% 75%, 50px 100%, 0 100%);
    clip-path: polygon(0 0, 100% 0, 100% 75%, 50px 100%, 0 100%);
    min-height: 26vw;
}
@media (max-width:960px) {
    .secondRowWrapper {
        -webkit-clip-path: polygon(0 0, 100% 0, 100% 85%, 50px 100%, 0 100%);
        clip-path: polygon(0 0, 100% 0, 100% 85%, 50px 100%, 0 100%);
        padding-bottom: 140px!important;
    }
    .firstRow {
        border-bottom: 2px solid #3B3B3B;
        padding-bottom: 24px;
    }
}
@media (max-width:960px) {
    .secondRowWrapper {
        -webkit-clip-path: polygon(0 0, 100% 0, 100% 95%, 50px 100%, 0 100%);
        clip-path: polygon(0 0, 100% 0, 100% 95%, 50px 100%, 0 100%);
    }
}
h1, h2 {
    color: #fff;
}
.secondRowIcon {
    max-width: 180px;
}
</style>