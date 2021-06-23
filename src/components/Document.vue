<template>
  <div class="row">
    <div class="col-25">
    <label>{{ msg }}</label></div>
  <div class="col-75">
    <select id="document" v-model="selected">
      <option disabled value="">Выберите один из вариантов</option>
      <option>Паспорт</option>
      <option>Свидетельство о рождении</option>
      <option>Вод. удостоверение</option>
    </select>
  </div>  </div>
</template>

<script>
  export default {
  name: 'Document',
  props: {
  msg: String
}
}
</script>

<style scoped>

</style>