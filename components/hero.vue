<template>
  <v-img
    :aspect-ratio="16/9"
    src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
    max-height="600"
  >
    <!-- <v-row align="center" class="lightbox white--text pa-2 fill-height"> -->
    <!-- <v-col>
        <div class="body-1">heyfromjonathan@gmail.com</div>
      </v-col>
    </v-row>-->
    <v-container class="fill-height">
      <div class="fill-height d-flex flex-column">
        <!-- <v-row class="flex-column pa-2"> -->
        <div class="d-flex flex-column justify-center white--text pa-2 fill-height">
          <div class="display-1 font-weight-bold mb-8">
            Every Child deserves the
            <br />best tutors, We care for your
            <br />learning needs
          </div>
          <div class="body-1">
            <v-btn color="success">Request for tutor</v-btn>
            <v-btn color="success" outlined>Become our partner</v-btn>
          </div>
        </div>
        <v-row align="end" class="lightbox white--text pa-2">
          <v-col>
            <div class="body-1 text-center">
              <v-icon>mdi-check-circle</v-icon><small>100% Satisfaction Guaranteed</small>
            </div>
          </v-col>
          <v-col>
            <div class="body-1 text-center"><v-icon>mdi-check-circle</v-icon><small>We care for all your learning needs</small></div>
          </v-col>
          <v-col>
            <div class="body-1 text-center"><v-icon>mdi-check-circle</v-icon><small>We find you best suited Tutor in less than 48 hrs</small></div>
          </v-col>
        </v-row>
        <!-- </v-row> -->
      </div>
    </v-container>
  </v-img>
</template>

<script>
export default {
  name: "hero"
};
</script>

<style>
</style>