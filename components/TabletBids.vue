<template>
  <v-container
    class="tabletBidsWrapper"
  >
      <v-row>
          <v-col
            cols=7
          >
            <v-img
                lazy-src="img/bidsList.png"
                src="img/bidsList.gif"
                class="tabletGif"
            ></v-img>
          </v-col>
          <v-col
            cols=5
          >
            <h2
                class="text-h4"
            >Join hundreds of users and bid on thousands of shipments today
            </h2>
            <p>Our bidding platform lets you have instant access to thousands of moves with the opportunity to service our Fortune 500 corporate customers. Shipments are posted hourly and are powered by our top-notch technology that makes the bidding process quick and seamless.</p>
            <div
                class="mainButtonSignUp"
            >Sign Up Now
            </div>
          </v-col>
      </v-row>
      <v-img
        src="/img/testimonialsDots.svg"
        width="150"
        class="testimonialDots"
      ></v-img>
  </v-container>
</template>

<script>
export default {

}
</script>

<style scoped>
  .tabletGif {
      margin-top: -100px;
      position: relative;
      z-index: 9;
      -webkit-box-shadow: -11px 11px 38px 5px rgba(114,114,114,0.6); 
      box-shadow: -11px 11px 38px 5px rgba(114,114,114,0.6);
      border-radius: 40px;
  }
  .testimonialDots {
    position: absolute;
    bottom: -48px;
    left: 80px;
  }
  .tabletBidsWrapper {
    position: relative;
  }
</style>