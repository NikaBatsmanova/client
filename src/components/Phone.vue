<template>
  <div class="phone">
    <label>Телефон</label>
    <input id="phone" size="30" type="text"  v-model="phone">
  </div>
</template>

<script>
  export default {
  name: 'Phone',
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
.phone {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>