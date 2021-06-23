<template>
  <div class="row">
    <div class="col-25">
    <label>{{ msg }}</label></div>
  <div class="col-75">
    <select id="doctor" v-model="selected">
      <option disabled value="">Выберите один из вариантов</option>
      <option>Иванов</option>
      <option>Захаров</option>
      <option>Чернышева</option>
    </select>
  </div>
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

</style>