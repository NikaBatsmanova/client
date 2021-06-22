<template>
  <div class="index">
    <label>{{ msg }}</label>
    <input autofocus id="index" onkeyup="" placeholder="" size="30" type="text">
  </div>
</template>

<script>
export default {
  name: 'AddressIndex',
  props: {
    msg: String
  }
}
</script>


<style scoped>
label {
  float:left;
  padding-right:30px;
}
input {  width: 60%;

  margin: 8px 0;
}
.index {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>