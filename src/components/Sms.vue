<template>
  <div class="row">
    <div class="col-25"><label>Не отправлять СМС</label>
    </div>
    <div class="col-75">
      <input id="sms" size="5" type="checkbox">
    </div>  </div>
</template>

<script>
  export default {
    name: 'Sms',
    props: {
      msg: String
    }
  }
</script>

<style scoped>

</style>