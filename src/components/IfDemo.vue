<template>
    <h2>v-if 条件渲染</h2>
    <div>
        <h3 v-if="isShow">This is a demo of v-if directive</h3>
        <button @click="isShow=!isShow">Toggle</button>
    </div>
    <div v-if="type === 'A'">Type is A</div>
    <div v-else-if="type === 'B'">Type is B</div>
    <div v-else>Type is not A or B</div>
</template>

<script>
export default{
    data(){
        return{
            isShow:true,
            type: 'A'
        }
    }    
}
</script>