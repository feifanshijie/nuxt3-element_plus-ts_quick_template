<template>
  <el-button @click="openVn">Hello world</el-button>
</template>
<script setup lang="ts">
import {  h } from 'vue'
import {ElMessage} from 'element-plus/lib';
const openVn = () => {
  ElMessage({
    message: h('p', null, [
      h('span', null, 'Message can be '),
      h('i', { style: 'color: teal' }, 'VNode'),
    ]),
  })
}
</script>
<style>
</style>
