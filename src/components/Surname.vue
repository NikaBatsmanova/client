<template>
  <div class="surname">
    <label>{{ msg }}</label>
    <input autofocus id="surname" onkeyup="" placeholder="" size="30" type="text"  v-model="surname">
  </div>
</template>

<script>
export default {
  name: 'Surname',
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
.surname {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>
