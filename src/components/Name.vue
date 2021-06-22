<template>
  <div class="name">
    <label>{{ msg }}</label>
    <input id="name" onkeyup="" placeholder="" size="30" type="text" v-model="name">
  </div>
</template>

<script>
export default {
  name: 'Name',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
label {
  float:left;
  padding-right:30px;
}
input {  width: 60%;

  margin: 8px 0;
}
.name {
  clear:both;
  text-align:right;
  line-height:25px;
}

</style>
