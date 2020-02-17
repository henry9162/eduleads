<template>
  <div class="text-center my-md-12 py-5">
      <h4 class="display-1 font-weight-bold">{{header}}</h4>
      <p class="body-1">{{subheader}}</p>
  </div>
</template>

<script>
export default {
    name:"sectionHeader",
    props:["header", "subheader"],
}
</script>

<style>

</style>