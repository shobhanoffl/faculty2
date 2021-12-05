<template>
<v-app>
  <new-post />
  <post-lay />
</v-app>
</template>

<script>
import NewPost from '../components/NewPost.vue'
import PostLay from '../components/PostLay.vue'

  export default {
    name: 'Home',
    components: {
      NewPost,PostLay
    },
  }
</script>

<style scoped>
@media only screen and (max-width: 900px){
  #app *{
    top: 25px;
  }
}
</style>

