<!--
 * @Author: fzf404
 * @Date: 2022-09-28 17:05:18
 * @LastEditors: fzf404 me@fzf404.art
 * @LastEditTime: 2022-11-09 19:51:14
 * @Description: loading 组件
-->
<template>
  <section v-show="show" class="flex-col-center modal z-30 space-y-2">
    <!-- 加载动画 -->
    <LoadSVG class="text-light load-rotating w-16" />
    <!-- 备注 -->
    <p class="text-intro" v-for="item in remark">{{ item }}</p>
  </section>
</template>

<script setup lang="ts">
import LoadSVG from '@/assets/layout/load.svg'

defineProps(['show', 'remark'])
</script>
