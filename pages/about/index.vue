<template>
  <div>
    <h2>about page</h2>
    <nuxt-child />
    <ul>
      <li>
        <nuxt-link :to="{name:'index'}">index page</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
    export default {
        name: "index"
    }
</script>

<style scoped>

</style>
