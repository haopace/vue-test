<script>
  import HelloWorld from './components/HelloWorld.vue'

  export default {
    name: 'App',
    data() {
      return {
        message: 'Hello Vue!',
        number : 11,
        is_ok : true,
        rawHtml : '<a href="https://www.baidu.com">百度一下</a>'
      }
    }
  }
</script>

<template>
  <h3>三级标题</h3>
  <p>{{ message }}</p>
  <p>{{ number + 1 }}</p>
  <p>{{ is_ok ? 'Yes' : 'No' }}</p>
  <p>{{ message.split('').reverse().join('') }}</p>
  <p v-html="rawHtml"></p>
</template>

