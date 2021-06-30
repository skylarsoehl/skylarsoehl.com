<template>
  <div>
    <NuxtLink :to="`project${url}`">{{ name }}</NuxtLink>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: '',
    },
    url: {
      type: String,
      default: '/',
    },
  },
}
</script>

<style></style>
