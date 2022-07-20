<script>
import Message from "./components/Message.vue";
import Row from "./components/Row.vue";
export default {
  name: "App",
  components: {Row, Message},
  data () {
    return {
      responses: [1,1,1,1],
      currentRow: [0,0,0,0]
    }
  },
  methods:
  {
    checkRow()
    {
      alert('plop');
    },
  }
}
</script>

<template>
  <main class="main">
    <div class="caseContainer">
      <Row :indexes="currentRow"></Row>
      <button @click="checkRow" id="btn">Valider</button>
    </div>
    <Message></Message>
  </main>
</template>

<style scoped>

.caseContainer {

  display: flex;
  flex-direction: row;
  gap: 1rem;

}

#btn {

  width: 5rem;
  cursor: pointer;
  background-color: lightblue;
  border-radius: 5px;
  border: none;
  margin-left: 2rem;


}

</style>
