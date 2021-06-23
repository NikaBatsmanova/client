<template>
  <div class="row">
    <div class="col-25">
    <label>{{ msg }}</label></div>
    <div class="col-75">
    <input id="dateOfIssue" size="30" type="date" v-model="dateOfIssue" required>
    </div>  </div>
</template>

<script>
export default {
  name: 'DateOfIssue',
  props: {
    msg: String
  }
}
</script>

<style scoped>

</style>