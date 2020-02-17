<template>
  <div>
      <v-row class="" dense>
        <v-col cols="12" :md="6">
          <p class="display-1 font-weight-bold ml-10">For Tutors</p>
          <timeline :steps="steps"></timeline>
          <v-btn color="primary my-5 ml-10">Become our partner</v-btn>
        </v-col>
        <v-col cols="12" :md="6" class="d-none d-md-block">
          <v-img
            src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
            class="fill-height"
          ></v-img>
        </v-col>
      </v-row>
      <div></div>
      <v-row dense>
        <v-col cols="12" :md="6">
          <v-img
            src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
            class="fill-height"
          ></v-img>
        </v-col>
    
        <v-col cols="12" :md="6">
          <p class="display-1 font-weight-bold ml-10">For Tutors</p>
          <timeline :steps="steps"></timeline>
          <v-btn color="primary my-5 ml-10">Become our partner</v-btn>
        </v-col>
      </v-row>
  </div>
</template>

<script>
import step from "./step";
import timeline from "./timeline";
export default { 
  components: {
    step,
    timeline
  },
  data() {
    return {
      steps: [
        {
          headline: "Apply as a Tutor",
          description:
            "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started."
        },
        {
          headline: "Get tested",
          description:
            "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started."
        },
        {
          headline: "Start earning",
          description:
            "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started."
        }
      ]
    };
  }
};
</script>

<style>
</style>