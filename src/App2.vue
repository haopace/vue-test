<template>
  <div v-bind:id="dynamicId" v-bind:class="dynamicClass">Appid</div>
  <button :disabled="!isShow">Click me</button>
  <div v-if="isShow">能够显示吗？</div>
  <div v-else>不能显示</div>

  <div v-if="type === 'A'">A</div>
  <div v-else-if="type === 'B'">B</div>
  <div v-else-if="type === 'C'">C</div>
  <div v-else>D</div>
  <div v-show="isShow">能够显示吗？</div>
</template>

<script>

  export default {
    data() {
      return {
        dynamicId: 'app123',
        dynamicClass: 'app-class',
        isShow: true,
        type: 'AB'
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