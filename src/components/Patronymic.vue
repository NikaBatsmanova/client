<template>
  <div class="patronymic">
    <label>{{msg}}</label>
    <input id="patronymic" onKeyUp="" placeholder="" size="30" type="text">
  </div>
</template>

<script>
  export default {
  name: 'Patronymic',
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
.patronymic {
  clear:both;
  text-align:right;
  line-height:25px;
}

</style>
