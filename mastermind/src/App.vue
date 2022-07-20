<script setup>
import Case from "./components/Case.vue";
import Message from "./components/Message.vue";
</script>

<template>
  <main>
    <div class="caseContainer">
      <Case></Case>
      <Case></Case>
      <Case></Case>
      <Case></Case>
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
