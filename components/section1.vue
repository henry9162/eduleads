<template>
  <div>
    <sectionHeader :header="header" :subheader="subheader"></sectionHeader>
    <v-row>
      <v-col cols="12" :md="4" :sm="6" v-for="(item, index) in cards" :key="index">
        <textCard :headline="item.headline" :subtitle="item.subtitle" :action="item.action"></textCard>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import textCard from "./textCard";
import sectionHeader from "./sectionHeader";
export default {
  name: "section1",
  components: {
    textCard,
    sectionHeader
  },
  data: () => ({
    header: "We bring learning solutions to your home",
    subheader: "We care for all your learning needs",
    cards: [
      {
        headline: "Nursery/KG",
        subtitle: "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      },
      {
        headline: "Primary",
        subtitle: "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      },
      {
        headline: "Junior Secodary",
       subtitle: "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      },
      {
        headline: "Secondary School",
          subtitle: "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      },
      {
        headline: "SSCE(WAEC/NECO)",
           subtitle: "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      },
      {
        headline: "JAMB/PUME",
          subtitle: "Passionate about sharing your knowledge to other designers? Join us in sharing your knowledge while earning as you do so. Click on the learn more button to get started.",
        action: "Request tutor"
      }
    ]
  })
};
</script>

<style>
</style>