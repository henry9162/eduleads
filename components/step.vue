<template>
  <div>
    <h6>{{heading}}</h6>
    <p>{{description}}</p>
  </div>
</template>

<script>
export default {
    name: "step",
    props: ["heading", "description"]
};
</script>

<style>
</style>