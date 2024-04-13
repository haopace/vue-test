<template>
    <h2>v-list列表渲染</h2>
    <h3>简单列表</h3>
    <div v-for="(item, index) in items" :key="index">{{ item }}-{{ index }}</div>
    <h3>对象列表</h3>
    <div v-for = "person of data" :key="person.age">{{ person.id }} - {{ person.name }}</div>
    <h3>简单对象</h3>
    <div v-for = "(value,key,index) in useInfo">{{ value }}-{{ key }}-{{ index }}</div>
</template>

<script>
export default {
    data() {
        return {
            items: ['apple', 'banana', 'orange'],
            data:[{'id':1,'name':'张三','age':29},{'id':2,'name':'李四','age':25},{'id':3,'name':'王五','age':28}] ,
            useInfo:{
                name: '季沧海',
                age: 2000,
                sex: '男'
            }
        }
    },
}
</script>