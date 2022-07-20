<template>
    <div :style="{'background-color': color}" :class="{'shadow': isShadow}" class="case"></div>

</template>

<script>
export default {
  name: "Case",
  data() {
    return {
      color: "blue",
      isShadow: true,
    }
  }
}
</script>

<style scoped>

.case {

  padding: 2rem;
  border: solid 1px white;
  cursor: pointer;

}

.shadow {

  box-shadow: 5px 5px 5px white;

}

</style>