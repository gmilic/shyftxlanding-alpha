<template>
  <v-app dark>
    <v-app-bar
      absolute
      color="#222222"
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

      

      <v-toolbar-items class="hidden-sm-and-down justify-start">
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

      <div class="toolbar-buttons">
        <v-btn
          class="mx-4 px-12 hidden-sm-and-down"
          href="#"
          outlined
          color="#fff"
        >
          Log in
        </v-btn>
        <v-btn
          class="mx-4 px-12 hidden-sm-and-down"
          href="#"
          color="#EB344A"
          dark
        >
          Sign Up Now
        </v-btn>
      </div>

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
      <v-container>
        <v-row>
          <v-col
            cols=3
          >
            <v-img
              class="mx-2"
              src="/img/ShyftX_logo.svg"
              max-height="40"
              max-width="300"
              contain
            ></v-img>
          </v-col>
          <v-col
            cols=3
          >
            <h5
              class="text-h6 mt-2"
            >Company</h5>
            <a href="#" class="my-4">About Us</a>
            <a href="#" class="my-4">Careers</a>
            <a href="#" class="my-4">Press</a>
            <a href="#" class="my-4">Blog</a>
          </v-col>
          <v-col
            cols=3
          >
            <h5
              class="text-h6 mt-2"
            >Partners</h5>
            <a href="#" class="my-4">Corporate Relocation</a>
            <a href="#" class="my-4">Relocation Management</a>
            <a href="#" class="my-4">Moving Pros</a>
          </v-col>
          <v-col
            cols=3
          >
            <h5
              class="text-h6 mt-2"
            >Information</h5>
            <a href="#" class="my-4">Contact Us</a>
            <a href="#" class="my-4">Terms and Conditions</a>
            <a href="#" class="my-4">Privacy Policy</a>
          </v-col>
        </v-row>
        <v-row>
          <v-col
            cols=12
            class="d-flex flex-row-reverse"
          >
            <a href="#"><img src="img/footerIconFacebook.svg" /></a>
            <a href="#"><img src="img/footerIconTwitter.svg" /></a>
            <a href="#"><img src="img/footerIconInstagram.svg" /></a>
          </v-col>
          <v-col
            cols=12
          >
          <hr />
          <div class="footerCopyright">
            2015 - {{ new Date().getFullYear() }} Shyft, Inc.
          </div>
          </v-col>
        </v-row>
      </v-container>
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
    background: url('/img/footerBg.png'), linear-gradient(171.19deg, #010101 47.37%, rgba(1, 1, 1, 0) 159.24%);
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center right;
    min-height: 500px;
    padding-top: 80px;

  }

  .appFooter h5,
  .appFooter p,
  .appFooter a {
    color: #fff;
    text-decoration: none;
  }
  .appFooter a {
    display: block;
  }
  .appFooter a img {
    margin: 0 10px;
    width: 40px;
  }
  .appFooter hr {
    color: #C9C9C9;
  }
  .footerCopyright {
    color: #C9C9C9;
    margin-top: 16px;
  }
  @media (min-width: 961px) {
    .toolbar-buttons {
      position: absolute;
      right: 30px;
    }
  }
</style>