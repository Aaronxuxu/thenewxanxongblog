<template>
  <div class="header">
    <el-avatar :size="60" :src="circleUrl" />
    <div class="header-title">徐轩雄</div>
  </div>
</template>

<script lang="ts" setup>
import { reactive, toRefs } from 'vue'

const state = reactive({
  circleUrl: 'https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png',
  squareUrl: 'https://cube.elemecdn.com/9/c2/f0ee8a3c7c9638a54940382568c9dpng.png',
  sizeList: ['small', '', 'large'] as const
})

const { circleUrl } = toRefs(state)
</script>

<style lang="less" scoped>
.header {
  display: flex;
  gap: 15px;
  align-items: center;
  transition: var(--transition-1);
  .header-title {
    font-size: 24px;
    font-weight: 700;
    letter-spacing: 1px;
  }
  @media (max-width: 594px) {
    flex-direction: column;
  }
}
</style>