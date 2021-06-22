<template>
  <div class="document">
    <label>{{ msg }}</label>
    <select id="document" v-model="selected">
      <option disabled value="">Выберите один из вариантов</option>
      <option>Паспорт</option>
      <option>Свидетельство о рождении</option>
      <option>Вод. удостоверение</option>
    </select>
  </div>
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
label {
  float: left;
  padding-right: 30px;
}

select {
  width: 60%;

  margin: 8px 0;
}

.document {
  clear: both;
  text-align: right;
  line-height: 25px;
}
</style>