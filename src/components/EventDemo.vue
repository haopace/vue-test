<template>
    <h2>内联事件处理器</h2>
    <div>Count is {{ count }}</div>
    <button v-on:click="count++">Add 1</button>
    <br/>
    <!-- @click 是v-on:click的简写 -->
    <button @dblclick="count+=2">双击加2</button>
    <br/>
    <h3>方法触发事件</h3>
    <button @click="handleClick">Add 3</button>
</template>

<script>
export default {
    name: 'EventDemo',
    data() {
        return {
           count: 0
        }
    },
    //定义方法的触发事件
    methods: {
        handleClick() {
            this.count += 3;
        }
    }
}
</script>

