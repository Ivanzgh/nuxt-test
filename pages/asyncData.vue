<template>
    <div>
      <h2>年龄：{{this.user.age}}</h2>
      <h2>爱好：{{this.user.interest}}</h2>
    </div>
</template>

<script>
  import axios from 'axios'
    export default {
        name: "asyncData",
      data() {
          return {
            user : {}
          }
      },
      async asyncData() {
          let {data} = await axios.get('https://api.myjson.com/bins/bucvi')
          return {user : data}
      }
    }
</script>

<style scoped>

</style>
