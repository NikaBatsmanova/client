<template>
  <div class="date">
    <label>{{ msg }}</label>
    <input id="dateofbirth" size="30" type="date" v-model="date">
  </div>
</template>

<script>
export default {
  name: 'DateOfBirth',
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
.date {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>