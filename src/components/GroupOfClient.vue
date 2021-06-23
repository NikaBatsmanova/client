<template>
  <div class="row">
    <div class="col-25">
      <label>{{msg}}</label></div>
    <div class="col-75"><select  multiple id="group" v-model="group" required>
      <option>VIP</option>
      <option>Проблемные</option>
      <option>ОМС</option>
    </select></div>
  </div>
</template>

<script>
  export default {
  name: 'GroupOfClient',
  props: {
  msg: String
}
}
</script>

<style scoped>

</style>