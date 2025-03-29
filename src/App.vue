<template>
  <a-config-provider :locale="zhCN" :theme="{ algorithm: app.algorithm }">
    <Home/>
  </a-config-provider>
</template>

<script setup>
import zhCN from "ant-design-vue/es/locale/zh_CN";
import Home from "./views/Home.vue";
import { app } from "./store";

app.initBackgroundColor();
</script>
