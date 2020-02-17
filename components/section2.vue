<template>
  <div>
    <sectionHeader :header="header" :subheader="subheader"></sectionHeader>
    <v-row>
      <v-col
        class="text-center"
        cols="12"
        :sm="6"
        :md="4"
        v-for="(item, index) in cards"
        :key="index"
      >
        <imageCard
          :src="item.src"
          :headline="item.headline"
          :description="item.description"
          :action="item.action"
        ></imageCard>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import imageCard from "./imageCard";
import sectionHeader from "./sectionHeader";

export default {
  name: "section2",
  components: {
    imageCard,
    sectionHeader
  },
  data: () => ({
    header: "Certified and Verified Teachers",
    subheader: "Because your security and peace of mind is paramount to us",
    cards: [
      {
        src: "https://cdn.vuetifyjs.com/ir",
        headline: "International Exams",
        description:
          "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      },
      {
        src: "https://cdn.vuetifyjs.com/ir",
        headline: "Secondary School Exams",
        description:
          "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      },
      {
        src: "https://cdn.vuetifyjs.com/ir",
        headline: "Primary School Exams",
        description:
          "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      }
    ]
  })
};
</script>

<style>
</style>