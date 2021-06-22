<template>
  <div class="doctor">
    <label>{{ msg }}</label>
    <select id="doctor" v-model="selected">
      <option disabled value="">Выберите один из вариантов</option>
      <option>Иванов</option>
      <option>Захаров</option>
      <option>Чернышева</option>
    </select>
  </div>
</template>

<script>
  export default {
  name: 'Doctor',
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
select {  width: 60%;

  margin: 8px 0;
}
.doctor {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>