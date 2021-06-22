<template>
  <a class="gradient-button" href="">Submit</a>
</template>

<script>
export default {
  name: "Validate"
}
</script>

<style scoped>
.gradient-button {
  text-decoration: none;
  display: inline-block;
  color: white;
  padding: 7px 7px;
  margin: 10px 20px;
  border-radius: 10px;
  font-family: 'Montserrat', sans-serif;
  text-transform: uppercase;
  letter-spacing: 2px;
  background-image: linear-gradient(to right, #FFB6C1 0%, #F08080 51%, #DC143C 100%);
  background-size: 200% auto;
  box-shadow: 0 0 20px rgba(0, 0, 0, .1);
  transition: .5s;
}

.gradient-button:hover {
  background-position: right center;
}
</style>