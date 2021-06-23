<template>
  <div class="row">
    <div class="col-25">
    <label>Телефон</label></div>
    <div class="col-75">
    <input id="phone" size="30" type="text"  v-model="phone">
  </div>  </div>
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

</style>