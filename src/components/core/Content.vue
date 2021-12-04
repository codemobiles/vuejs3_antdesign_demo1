<template>
  <a-layout-content
    :style="{
      margin: '24px 16px',
      padding: '24px',
      background: '#fff',
      minHeight: '280px',
    }"
  >
    <div>
      <h1>Ok</h1>
      <a-button type="primary">Primary Button</a-button>
      <a-button>Default Button</a-button>
      <a-button type="dashed">Dashed Button</a-button>
      <a-button type="text">Text Button</a-button>
      <a-button type="link">Link Button</a-button>
    </div>
  </a-layout-content>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    return {};
  },
});
</script>
