<!--
 * @Author: your name
 * @Date: 2022-04-01 23:00:56
 * @LastEditTime: 2022-04-23 08:27:58
 * @LastEditors: Please set LastEditors
 * @Description: 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 * @FilePath: \vitesse\src\pages\index.vue
-->
<script setup lang="ts">
import { useUserStore } from '~/stores/user'

const router = useRouter()
const go = () => {
  router.push('/Foo')
}
</script>

<template>
  <div>
    Index
    <div>
      <button
        btn m-3 text-sm
        @click.stop="go"
      >
        go
      </button>
    </div>
    <FloatingProxy w-50 h-50 rounded-10 />
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
