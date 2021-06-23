<template>
  <div class="row">
    <div class="col-25">
    <label>{{ msg }}</label></div>
    <div class="col-75">
    <input id="house" onkeyup="" placeholder="" size="30" type="text">
    </div>  </div>
</template>

<script>
export default {
  name: 'House',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>