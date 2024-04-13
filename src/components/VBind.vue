<template>
    <div v-bind:id="dynamicId" v-bind:class="dynamicClass">Appid</div>
    <button :disabled="!isShow">Click me</button>
    <ifDemo />
</template>
  
  <script>
    export default {
      data() {
        return {
          dynamicId: 'app123',
          dynamicClass: 'app-class',
          isShow: false
        }
    }
  }
  </script>
  
  <style>
    .app-class {
        color:red;
        font-size: 20px;
    }
  </style>