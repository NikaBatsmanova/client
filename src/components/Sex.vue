<template>
  <div class="row">
    <div class="col-25">
    <label>Пол</label></div>
  <div class="col-75">
    <select id="sex" v-model="selected">
      <option disabled value="">Выберите один из вариантов</option>
      <option>Женский</option>
      <option>Мужской</option>
    </select>
  </div>  </div>
</template>

<script>
export default {
  name: 'Sex',
  props: {
    msg: String
  }
}
</script>

<style scoped>

</style>