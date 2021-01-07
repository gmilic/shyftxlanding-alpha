<template>
  <div>
      <v-container
        class="my-16"
      >
          <v-row>
              <v-col
                cols=12
              >
                <h3
                    class="howShyftxWordTitle"
                >
                    How ShyftX Works for You
                </h3>
              </v-col>
          </v-row>
      </v-container>
      <v-container
        fluid
        class="howShyftxWorkBg"
      >
        <v-container>
            <v-row
                justify="center"
            >
                <v-col
                    cols=4
                >
                    <h2
                        class="text-h3 my-4"
                    >
                        Bid for moves in three easy clicks
                    </h2>
                    <p>
                        Bid on all kinds of moves and shipments in three simple steps. Just log onto the ShyftX platform, select your move or carshipment and enter your bid details. We focus on finding leads so that you can focus on getting full trucks on the road. 
                    </p>
                    <div
                        class="mainButtonSignUp"
                    >Sign Up For Free
                    </div>
                </v-col>
                <v-col
                    cols=3
                    class="d-flex flex-row-reverse"
                >
                    <v-img
                        src="/img/bid-window-v2.gif"
                        lazy-src="/img/bid-window-v2.png"
                        class="bidWindow"
                    ></v-img>
                </v-col>
            </v-row>
        </v-container>
      </v-container>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.howShyftxWordTitle {
    font-size: 6em;
    line-height: 1.1;
}
.bidWindow{
    -webkit-box-shadow: -5px 4px 15px 5px rgba(0,0,0,0.5); 
    box-shadow: -5px 4px 15px 5px rgba(0,0,0,0.5);
}
.howShyftxWorkBg {
    background-image: url('/img/howShyftxWorksBg.png');
    background-repeat: no-repeat;
    background-position: center right;
    background-size: contain;
}
</style>