<script setup>
import Message from "./components/Message.vue";
import Row from "./components/Row.vue";
</script>

<template>
  <main>
    <div class="caseContainer">
      <Row></Row>
      <button id="btn">Valider</button>
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

}

</style>
