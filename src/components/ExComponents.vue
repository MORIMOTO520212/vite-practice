<script setup lang="ts">

interface FileData {
  dataUrl: string | undefined,
  name: string | undefined,
}
interface Props {
    data: FileData
}
const props = defineProps<Props>()

</script>
<template>
    <p>ExComponents => {{ props.data.dataUrl }}</p>
</template>