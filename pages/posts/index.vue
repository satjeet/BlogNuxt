<template>
  <div class="posts-page">
    <section class="posts-list">
      <PostList/>
    </section>
  </div>
</template>


<script>
import PostList from '~/components/Posts/PostList.vue'


export default {
  components:{
    PostList
  }
}
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  text-align: center;
}

</style>
