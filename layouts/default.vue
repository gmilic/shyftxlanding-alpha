<template>
  <v-app dark>
    <v-app-bar
      absolute
      color="rgba(18, 33, 32, 0.64)"
      elevate-on-scroll
      style="position:fixed"
    >
      <v-img
        class="mx-2"
        src="/img/ShyftX_logo.svg"
        max-height="40"
        max-width="160"
        contain
      ></v-img>

      <v-spacer></v-spacer>

      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn
          href="#"
          color="transparent"
          dark
          elevation="0"
        >
        How it works
        </v-btn>        <v-btn
          href="#"
          color="transparent"
          dark
          elevation="0"
        >
        Pricing
        </v-btn>        <v-btn
          href="#"
          color="transparent"
          dark
          elevation="0"
        >
        Resources
        </v-btn>
      </v-toolbar-items>


        <v-btn
          class="mx-4 hidden-sm-and-down"
          href="#"
          outlined
          color="#fff"
        >
          Log in
        </v-btn>
        <v-btn
          class="mx-4 hidden-sm-and-down"
          href="#"
          color="#EB344A"
          dark
        >
          Get A Free Demo
        </v-btn>


      <v-app-bar-nav-icon
        class="hidden-md-and-up"
        dark
        @click="drawer = true"
      >
        
      </v-app-bar-nav-icon>
    </v-app-bar>
    <v-main>

        <nuxt />

    </v-main>
    <div
      class="appFooter"
    >
    </div>
  </v-app>
</template>

<script>
export default {
  data () {
    return {}
  }
}
</script>

<style scope>
  .appFooter {
    background-color: #121212;
    background-image: url('/img/bg-footer.png');
    background-position: center top;
    background-repeat: no-repeat;
    height: 650px;
    background-size: cover;
  }
</style>