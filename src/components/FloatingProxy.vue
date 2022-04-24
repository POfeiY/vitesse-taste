<!--
 * @Author: your name
 * @Date: 2022-04-23 00:06:30
 * @LastEditTime: 2022-04-24 23:46:10
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vitesse\src\components\FloatingProxy.vue
-->

<script setup lang="ts">
import { el, metaData } from '~/composables/floating'
const props = defineProps<{
  modelValue?: boolean
}>()
const attrs = useAttrs()

metaData.props = props
metaData.attrs = attrs

const proxyEle = ref<HTMLElement | null>(null)
onMounted(() => {
  el.value = proxyEle.value
})
</script>
<template>
  <div ref="proxyEle" bg-gray-400:10>
    <slot />
  </div>
</template>
