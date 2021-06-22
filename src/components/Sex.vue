<template>
  <div class="sex">
    <label>Пол</label>
    <select id="sex" v-model="selected">
      <option disabled value="">Выберите один из вариантов</option>
      <option>Женский</option>
      <option>Мужской</option>
    </select>
  </div>
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
label {
  float:left;
  padding-right:30px;
}
select {  width: 60%;

  margin: 8px 0;
}
.sex {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>