<template>
  <span>{{ msg }}</span>
</template>

<script>
export default {
  name: "Message",
  data (){
    return{
      msg: "Mastermind",
    }
  }
}
</script>

<style scoped>

span{

  color: white;

}

</style>