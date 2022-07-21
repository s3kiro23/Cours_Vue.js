<template>
  <main class="main">
    <div class="caseContainer">
      <Row :indexes="currentRow" @clickCase="colorChanged"></Row>
      <button @click="checkRow" class="btn">Valider</button>
    </div>
    <Message></Message>
  </main>
</template>

<script>
import Message from "./components/Message.vue";
import Row from "./components/Row.vue";
import mock from "./assets/mock";

export default {
  name: "App",
  components: {Row, Message},
  data() {
    return {
      mock,
      responses: [1, 1, 1, 1],
      currentRow: [1, 0, 3, 0],
    };
  },
  methods: {
    checkRow() {
      alert("plop");
    },

    colorChanged(id){
      let color = this.currentRow[id];
      color++;
      if (this.index >= mock.colors.length) {
        color = 0;
      }
      this.currentRow[id] = color;
    }
  }
}
</script>

<style scoped>

.caseContainer {

  display: flex;
  flex-direction: row;
  gap: 1rem;

}

.btn {

  width: 5rem;
  cursor: pointer;
  background-color: lightblue;
  border-radius: 5px;
  border: none;
  margin-left: 2rem;


}

</style>
