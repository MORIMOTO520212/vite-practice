<script setup lang="ts">
import { reactive } from 'vue';
import ExComponents from './components/ExComponents.vue';


interface FileData {
  dataUrl: string | undefined,
  name: string | undefined,
}
const fileData: FileData = reactive({
  dataUrl: undefined,
  name: undefined,
});
fileData.dataUrl = "https://example.com";
fileData.name = "example";
</script>

<template>
  <p>fileData.dataUrl = {{ fileData.dataUrl }}</p>
  <ExComponents :data="fileData" />
</template>