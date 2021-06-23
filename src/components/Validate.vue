<template>
  <div class="row">
  <input type="submit" value="Submit">
    </div>
</template>

<script>
export default {
  name: "Validate"
}
</script>

<style scoped>
input[type=submit] {
  background-color: #F08080;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
  text-align: center;
  margin-top: 12px;
}

input[type=submit]:hover {
  background-color: #DC143C;
}
</style>