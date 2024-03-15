<template>
  <v-footer dark padless>
    <v-card flat tile class="black white--text py-5 px-5 text-center" width="100%">
        <v-row>
            <v-col cols="12" sm="4">
              <v-card-text class="white--text pt-2">
                <v-btn icon>
                  <v-icon color="#A7121D">mdi-account</v-icon>
                </v-btn>
              </v-card-text>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card-text class="pt-2">
                <a href="https://github.com/Kraken-ops">
                <v-btn  class="mx-1 white--text" icon>
                  <v-icon size="24px">mdi-github</v-icon>
                </v-btn>
              </a>
                <a href="https://www.facebook.com/Ciarra.la.de.Rebellion/">
                <v-btn  class="mx-1 white--text" icon>
                  <v-icon size="24px">mdi-facebook</v-icon>
                </v-btn>
              </a>
              <a href="https://www.linkedin.com/in/priyansu-dey-2001/">
                <v-btn  class="mx-1 white--text" icon>
                  <v-icon size="24px">mdi-linkedin</v-icon>
                </v-btn>
              </a>
                <a href="https://www.instagram.com/this_is_kraken/?fbclid=IwAR0cKaZxKTdc9nK3ZmqW2QDDE4wfJAef7y6_tXHz0-nzotuZC--TvhCt7LQ">
                <v-btn  class="mx-1 white--text" icon>
                  <v-icon size="24px">mdi-instagram</v-icon>
                </v-btn>
              </a>
              <a href="">
                <v-btn  class="mx-1 white--text" icon>
                  <v-icon size="24px">mdi-twitter</v-icon>
                </v-btn>
              </a>
              </v-card-text>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card-text class="pt-2">
                <v-btn class="mx-1 white--text" icon>
                  <v-icon color="#A7121D">mdi-heart</v-icon>
                </v-btn>
                Created by Priyanshu Dey
              </v-card-text>
            </v-col>
        </v-row>
    </v-card>
  </v-footer>
</template>

<script>
export default {
data() {
  return {
    icons:["mdi-facebook","mdi-twitter","mdi-linkedin","mdi-instagram"]
  }
},
}
</script>

<style>

</style>