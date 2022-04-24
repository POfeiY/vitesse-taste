<!--
 * @Author: your name
 * @Date: 2022-04-22 07:15:32
 * @LastEditTime: 2022-04-25 00:21:38
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vitesse\src\pages\Foo.vue
-->
<script setup lang="ts">
import FloatingProxy from '~/components/FloatingProxy.vue'
const router = useRouter()
const back = () => {
  router.back()
}
</script>
<template>
  <div>Foo</div>
  <button
    btn m-3 text-sm
    @click="back"
  >
    go soo
  </button>
  <div m80>
    <FloatingProxy w-50 h-50 rounded="1/2" />
  </div>
</template>
