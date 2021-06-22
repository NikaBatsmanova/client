<template>
  <div class="sms">
    <input id="sms" size="30" type="checkbox">
    <label>Не отправлять СМС</label>
  </div>
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
label {
  float:left;
  padding-right:30px;
}
input {

  margin: 8px 0;
}
.sms {
  clear:both;
  text-align:right;
  line-height:25px;
}
</style>