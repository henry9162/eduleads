<template>
  <v-layout
    column
  >
    <hero></hero>
    <v-container>
      <section1></section1>
      <imageSection></imageSection>
      <section2></section2>
    </v-container>
  </v-layout>
</template>

<script>
import hero from '~/components/hero.vue'
import section1 from '~/components/section1.vue'
import section2 from '~/components/section2.vue'
import imageSection from '~/components/imageSection.vue'

export default {
  components: {
    hero,
    section1,
    section2,
    imageSection,
  }
}
</script>
