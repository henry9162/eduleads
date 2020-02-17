<template>
        <v-timeline :align-top="alignTop" :dense="dense" :reverse="reverse">
        <v-timeline-item
          v-for="(item, index) in steps" :key="index"
          :fill-dot="fillDot"
          :hide-dot="hideDot"
          :icon="icon ? 'mdi-star' : ''"
          :icon-color=" iconColor ? 'deep-orange' : ''"
          :left="left"
          :right="right"
          :small="small"
        >
                <v-card-title class="headline">{{item.headline}}</v-card-title>
                <v-card-text>{{item.description}}</v-card-text>
        </v-timeline-item>
      </v-timeline>
</template>

<script>
export default {
    name: "timeline",
    props:["steps"],
  data() {
    return {
      alignTop: false,
      avatar: false,
      dense: true,
      fillDot: false,
      hideDot: false,
      icon: false,
      iconColor: false,
      left: false,
      reverse: false,
      right: true,
      small: true
    };
  }
}
</script>

<style scoped>
.v-timeline-item__divider{
    align-items:start !important;
}
</style>