<template>
  <v-dialog
      v-model="dialog"
      persistent
      max-width="400"
      max-height="400"
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn dark text v-bind="attrs"
          v-on="on">
                    know more
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
      </template>
      <v-card color="#1e1e1e" dark>
        <v-card-title class="text-h5">
          Use Google's location service?
        </v-card-title>
        <v-card-text>Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.</v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="blue darken-1"
            text
            @click="dialog = false"
          >
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
</template>

<script>
  export default {
    data () {
      return {
        dialog: false,
      }
    },
  }
</script>

<style>

</style>