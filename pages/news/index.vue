<template>
  <div>
    <h2>news page</h2>
    <ul>
      <li>
        <nuxt-link :to="{name:'index'}">index page</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name:'news-id',params:{id : 1},title: 'hello world'}">news-1</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name:'news-id',params:{id : 2},title: 'hello zgh'}">news-2</nuxt-link>
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
