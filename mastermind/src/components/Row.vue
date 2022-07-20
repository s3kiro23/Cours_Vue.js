<template>
  <Case v-for="i in 4" :key="i"></Case>
</template>

<script>

import Case from "./Case.vue"

export default {
  name: "Row",
  components: {Case}
}
</script>

<style scoped>

</style>