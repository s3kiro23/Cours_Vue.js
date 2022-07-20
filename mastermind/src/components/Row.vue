<template>
  <Case v-for="i in indexes.length"
        :key="i"
        :id="i"
        :index="indexes[i]"
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
    colorChanged(id){
      alert(this.id)
      /*this.$emit("clickCase", this.id)*/
    }
  }
}
</script>

<style scoped>

</style>