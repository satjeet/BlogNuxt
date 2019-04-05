<template lang="html">


  <section class="posts-list">
    <PostPreview
    id="1"
    title="hola"
     previewText="historia bonita"
     thumbnail="https://plumaslibres.com.mx/wp-content/uploads/2019/01/300px-Antennae_galaxies_xl.jpg" />
     <PostPreview
     id="2"
     title="Chao"
      previewText="historia mas bonita"
      thumbnail="https://plumaslibres.com.mx/wp-content/uploads/2019/01/300px-Antennae_galaxies_xl.jpg" />
      <PostPreview
      id="3"
      title="Aloha"
       previewText="no se me ocurre otra historia"
       thumbnail="https://plumaslibres.com.mx/wp-content/uploads/2019/01/300px-Antennae_galaxies_xl.jpg" />
  </section>
</template>

<script>
import PostPreview from '~/components/Posts/PostPreview.vue'

export default {
  components:{
    PostPreview
  }
}
</script>

<style scoped>

.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
