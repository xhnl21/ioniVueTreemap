<template>
  <!-- <chart /> -->
  <treemap />
</template>

<script>
import Chart from "../components/chart.vue";
import treemap from "../components/treemap.vue";
export default {
  name: "app",
  components: {
    Chart,
    treemap
  },
  methods: {
    handler() {
      var args = arguments;
      for (var arg of args) {
        if (arg instanceof Function) {
          arg();
        }
      }
    }
  }
};
</script>

<style scoped>
#container {
  min-width: 300px;
  max-width: 600px;
  margin: 0 auto;
}
</style>
