<template>
  <form @submit.prevent="onSave">
    <AppControlInput v-model="editedPost.author">Author Name</AppControlInput>

   <AppControlInput v-model="editedPost.title">Title</AppControlInput>

   <AppControlInput v-model="editedPost.thumbnailLink">Thumbnail Link</AppControlInput>

   <AppControlInput
             control-type="textarea"
             v-model="editedPost.content">Content</AppControlInput>

   <AppButton type="submit">Save</AppButton>

   <AppButton
             type="button"
             style="margin-left: 10px"
             btn-style="cancel"
             @click="onCancel">Cancel</AppButton>
  </form>
</template>

<script>
import AppControlInput from '~/components/UI/AppControlInput'
import AppButton from '~/components/UI/AppButton'

export default {
  components:{
    AppControlInput,
    AppButton
  },
  data(){
    return{
      editedPost:{
        author:'',
        title:'',
        thumbnailLink:'',
        content:'',
      }
    }
  },
  methods:{
    onSave(){
      //save the post
      console.log(this.editedPost);
    },
    onCancel(){
      //navegar hacia atras
      this.$router.push('/admin');
    }
  }
}
</script>

<style lang="css">
</style>
