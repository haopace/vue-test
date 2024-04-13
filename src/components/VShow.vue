<template>
    <h2>v-show 条件渲染 无论条件是否成立都会渲染</h2>
    <div v-show="show">能够看到我</div>
    <button @click="show = !show">切换显示</button>
</template>

<script>
export default {
    data() {
        return {
            show: true
        }
    }
}
</script>