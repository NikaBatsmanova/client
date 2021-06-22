<template>
  <div class="region">
    <label>{{ msg }}</label>
    <input autofocus id="region" onkeyup="" placeholder="" size="30" type="text">
  </div>
</template>

<script>
export default {
  name: 'Region',
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
.region {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>