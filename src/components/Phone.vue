<template>
  <div class="row">
    <div class="col-25">
    <label>Телефон</label></div>
    <div class="col-75">
      <div class="input-group">
        <span class="input-group-addon"></span>
        <input
            type="tel"
            v-model="phone"
            name="phone"
            id="phone"
            placeholder="7 (555) 555-5555"
            autocomplete="tel"
            maxlength="15"
            class="form-control"
            v-phone
            required
        />
      </div>
  </div>  </div>
</template>

<script>
import Vue from 'vue'
  export default {
  name: 'Phone',
  props: {
  msg: String
}
}
Vue.directive('phone', {
  bind(el) {
    function replaceNumberForInput(value) {
      let val = ''
      const x = value.replace(/\D/g, '').match(/(\d{0,1})(\d{0,3})(\d{0,3})(\d{0,4})/)

      if (!x[2] && x[1] !== '') {
        val = x[1] === '7' ? x[1] : '7' + x[1]
      } else {
        val = !x[3] ? x[1] + x[2] : x[1] + '(' + x[2] + ') ' + x[3] + (x[4] ? '-' + x[4] : '')
      }

      return val
    }

    function replaceNumberForPaste(value) {
      const r = value.replace(/\D/g, '')
      let val = r
      if (val.charAt(0) === '7') {
        val = '7' + val.slice(1)
      }
      return replaceNumberForInput(val)
    }

    el.oninput = function(e) {
      if (!e.isTrusted) {
        return
      }
      this.value = replaceNumberForInput(this.value)
    }

    el.onpaste = function() {
      setTimeout(() => {
        const pasteVal = el.value
        this.value = replaceNumberForPaste(pasteVal)
      })
    }

  }
})
</script>

<style scoped>

</style>