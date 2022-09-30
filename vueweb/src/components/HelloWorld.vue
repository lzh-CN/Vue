
<script>
import method from 'bluebird/js/release/method';
import { ref, onMounted } from 'vue'
import testJs from './test.js'

export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: 'lzh to Your Vue.js App',
      count: 1
    }
  },

  methods: {
    clickButton() {
      this.count++
    }
  }
}


onMounted(() => {
  console.log(`The initial count is ${count.value}.`)
})
</script>


<style scoped>
button {
  font-weight: bold;
}
</style>

<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>

    <button @click="clickButton">Count is: {{ count }}</button>
  </div>
</template>
