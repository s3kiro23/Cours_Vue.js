<template>
  <div>
    {{ msg }}
  </div>
  <input type="text" v-model="msg">
  <div>
    <img :src="msg" alt="pic">
  </div>
</template>

<script>
export default {
  name: "Message",
  data() {
    return {
      msg: "https://picsum.photos/200",
    }
  }
}
</script>

<style scoped>

span {

  color: white;

}

</style>