<template>
  <div class="row">
    <div class="col-25">
    <label>{{ msg }}</label></div>
  <div class="col-75">
    <input id="issuedBy" onkeyup="" placeholder="" size="30" type="text">
  </div>  </div>
</template>

<script>
export default {
  name: 'IssuedBy',
  props: {
    msg: String
  }
}
</script>

<style scoped>

</style>