<template>
    <div>
      <h2>news id is : {{$route.params.id}}</h2>
      <ul>
        <li>
          <nuxt-link :to="{name:'news'}">news page</nuxt-link>
        </li>
      </ul>
    </div>
</template>

<script>
    export default {
        name: "_id",
      //路由参数校验
      validate ({ params }) {
        // 必须是number类型
        return /^\d+$/.test(params.id)
      },
      data() {
          return {
            title : this.$route.params.title
          }
      },
      head() {
          return {
            title : this.title,
            meta : [
              {
                hid : 'description',
                name : 'news',
                content : 'this is news page'
              }
            ]
          }
      }
    }
</script>

<style scoped>

</style>
