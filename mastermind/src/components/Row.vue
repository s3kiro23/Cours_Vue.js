<template>
  <Case
      v-for="(i) in indexes.length"
      :key="i-1"
      :id="i-1"
      :index="indexes[i-1]"
      @changeColor="colorChanged"
  >
  </Case>
</template>

<script>

import Case from "./Case.vue"

export default {
  name: "Row",
  props: ["indexes"],
  components: {Case},
  methods: {
    colorChanged(caseID) {
      //alert(caseID);
      this.$emit("clickCase", caseID)
    }
  }
}
</script>

<style scoped>

</style>