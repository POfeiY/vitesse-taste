<!--
 * @Author: your name
 * @Date: 2022-04-22 07:19:38
 * @LastEditTime: 2022-04-23 00:27:49
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vitesse\src\pages\Soo.vue
-->
<script setup lang="ts">
const router = useRouter()
const goFoo = () => {
  router.push('/Foo')
}
</script>
<template>
  <div>Soo</div>
  <button
    btn m-3 text-sm
    @click="goFoo"
  >
    go foo
  </button>
  <FloatingProxy w-80 h-80 rounded-1 />
</template>
