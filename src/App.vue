<template>
  <a-layout style="min-height: 100vh">
    <!-- menu -->
    <Menu v-model:collapsed="collapsed" />
    <a-layout>
      <!-- heaer -->
      <Header v-model:collapsed="collapsed" />
      <!-- content -->
      <Content />
    </a-layout>
  </a-layout>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import Menu from "@/components/core/Menu.vue";
import Header from "@/components/core/Header.vue";
import Content from "@/components/core/Content.vue";
export default defineComponent({
  components: {
    Menu,
    Header,
    Content,
  },
  setup() {
    return {
      selectedKeys: ref<string[]>(["1"]),
      collapsed: ref<boolean>(false),
    };
  },
});
</script>
