<template>
  <NuxtLayout name="custom">
    <template #header> Some header template content. </template>

    The rest of the page
  </NuxtLayout>
</template>

<script setup>
export default {
  layout: 'custom',
}
</script>
