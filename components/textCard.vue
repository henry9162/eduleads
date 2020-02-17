<template>
  <v-card active-class="class"  tile>
    <div class="d-flex align-baseline">
        <div class="ma-2">
            <v-icon>mdi-application</v-icon>
            <p>dnik</p>
        </div>
        <div>
            <v-card-title class="headline">{{headline}}</v-card-title>
            <v-card-subtitle>{{subtitle}}</v-card-subtitle>
            <v-card-actions>
              <v-btn text color="success">{{action}}</v-btn>
            </v-card-actions>
        </div>
    </div>
  </v-card>
</template>

<script>
export default {
  props:["headline", "subtitle", "action"]
};
</script>

<style>
</style>