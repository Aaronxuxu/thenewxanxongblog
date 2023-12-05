<script setup lang="ts">
import { RouterView } from 'vue-router'
import footerIndexVue from './components/Footer/footerIndex.vue'
import pcHeader from '@/components/pcHeader/pcHeader.vue'
</script>

<template>
  <div class="main">
    <pcHeader />
    <RouterView />
  </div>
  <footerIndexVue />
  <el-backtop :right="30" :bottom="150" />
</template>

<style scoped>
.main {
  width: 80%;
  min-height: calc(100vh - 107px);
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding: 15px 5%;
  margin: 0 auto 50px;
  transition: var(--transition-1);
  @media (max-width: 1200px) {
    width: 95%;
    padding: 15px;
  }
}
</style>
