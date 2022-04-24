<!--
 * @Author: your name
 * @Date: 2022-04-22 07:22:13
 * @LastEditTime: 2022-04-25 00:11:03
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vitesse\src\components\TheImage.vue
-->
<script setup lang="ts">
const [toggle, changeTaggle] = useToggle(false)
</script>
<template>
  <div transition-all overflow-hidden>
    <img v-if="toggle" object-cover src="https://images.unsplash.com/photo-1640629071150-e5e978f63843?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80" @click.stop="changeTaggle">
    <img v-else object-cover src="https://images.unsplash.com/photo-1650582666861-1da18207c178?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80" @click.stop="changeTaggle">
  </div>
</template>
