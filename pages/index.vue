<template>
  <div>
    <h2>index page</h2>
    <div><img src="~static/avEUftE.png" alt=""></div>
    <ul>
      <li>
        <nuxt-link :to="{name:'index'}">index</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name:'news'}">news</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name:'about'}">about</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    components: {}
  }
</script>

<style>

</style>
