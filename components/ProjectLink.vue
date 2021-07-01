<template>
  <div>
    <NuxtLink class="project-link" :to="`project${url}`">{{ name }}</NuxtLink>
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

<style>
.project-link {
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: normal;
  font-size: 96px;
  line-height: 109.63%;
}
</style>
