<!--
 * @Author: your name
 * @Date: 2022-04-01 23:00:56
 * @LastEditTime: 2022-04-23 08:38:21
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vitesse\src\App.vue
-->
<script setup lang="ts">
import TheImage from './components/TheImage.vue'
// https://github.com/vueuse/head
// you can use this to manipulate the document head in any components,
// they will be rendered correctly in the html results with vite-ssg
useHead({
  title: 'Vitesse',
  meta: [
    { name: 'description', content: 'Opinionated Vite Starter Template' },
  ],
})
</script>

<template>
  <router-view />
  <FloatingContainer v-slot="props">
    <TheImage v-bind="props" />
  </floatingcontainer>
</template>
