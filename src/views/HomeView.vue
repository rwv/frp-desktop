<template>
  <div style="height: 100vh; position: relative" class="main-layout">
    <n-layout position="absolute">
      <n-layout-header style="height: var(--header-height); padding: 2em" bordered>
        FRP Desktop
      </n-layout-header>
      <n-layout
        has-sider
        position="absolute"
        style="top: var(--header-height); bottom: var(--footer-height)"
      >
        <n-layout-sider bordered content-style="padding: 2em;">Configs</n-layout-sider>
        <n-layout content-style="padding: 2em;"> Config Detail </n-layout>
      </n-layout>
      <n-layout-footer
        bordered
        position="absolute"
        style="height: var(--footer-height); padding: 2em"
      >
        Other
      </n-layout-footer>
    </n-layout>
  </div>
</template>

<script setup lang="ts">
import { NLayout, NLayoutHeader, NLayoutSider, NLayoutFooter } from 'naive-ui'
</script>

<style scoped>
.main-layout {
  --header-height: 5em;
  --footer-height: 5em;
}
</style>
