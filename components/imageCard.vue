<template>
  <VCard max-width="344">
      <VImg src="https://cdn.vuetifyjs.com/ir" height="200px">
      </VImg>
      <VCardTitle>
              <h3 class="headline">{{headline}}</h3>
      </VCardTitle>
              <v-card-text class="text-left body-1">{{description}}</v-card-text>
      <VCardActions>
          <VBtn text color="primary">{{action}}</VBtn>
      </VCardActions>
  </VCard>
</template>

<script>
export default {
    name:"imageCard",
    props:["src", "headline", "description", "action"]
}
</script>

<style>

</style>