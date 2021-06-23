<template>
  <div class="row">
    <div class="col-25">
    <label>{{msg}}</label></div>
    <div class="col-75">
    <input id="patronymic" onKeyUp="" placeholder="" size="30" type="text">
  </div>  </div>
</template>

<script>
  export default {
  name: 'Patronymic',
  props: {
  msg: String
}
}
</script>

<style scoped>

</style>
