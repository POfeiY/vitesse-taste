<!--
 * @Author: your name
 * @Date: 2022-04-23 00:24:07
 * @LastEditTime: 2022-04-25 00:09:42
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vitesse\src\components\FloatingContainer.vue
-->
<script setup lang="ts">
import type { StyleValue } from 'vue'
import { el, metaData } from '~/composables/floating'
const rect = ref<DOMRect>()
watch(el, (val) => {
  rect.value = val?.getBoundingClientRect()
}, { immediate: true })
const containerStyle = computed(() => ({
  position: 'fixed',
  transition: 'all .8s ease-in-out',
  top: `${rect.value?.top ?? 0}px`,
  left: `${rect.value?.left ?? 0}px`,
}))
</script>
<template>
  <div :style="containerStyle">
    <slot v-bind="{...metaData.attrs}" />
  </div>
</template>
