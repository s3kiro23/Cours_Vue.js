<template>
  <div @click="changeColor"
       :style="{'background-color': mock.colors[index]}"
       :class="{'shadow': isShadow}"
       class="case">
  </div>
</template>

<script>

import mock from "../assets/mock";

export default {
  name: "Case",
  data() {
    return {
      mock,
      isShadow: true,
      index: 0,
    }
  },
  methods:
      {
        changeColor() {

          this.index++;

          if (this.index >= mock.colors.length) {
            this.index = 0;
          }
          this.color = mock.colors[this.index]

        }
      }
};
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