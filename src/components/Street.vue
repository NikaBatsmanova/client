
<template>
  <div class="street">
    <label>{{ msg }}</label>
    <input autofocus id="street" onkeyup="" placeholder="" size="30" type="text">
  </div>
</template>

<script>
export default {
  name: 'Street',
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
.street {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>