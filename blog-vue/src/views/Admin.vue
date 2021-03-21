<template>
    <div>
        <CreateArticle @add="saveBlog" />
        <hr>
        <br>
        
        
        <!-- <PostBlog /> -->
        <ModifArticle :articles="articles" />
    </div>
    
</template>
<script>
// @ is an alias to /src
import CreateArticle from '@/components/CreateArticle.vue'
import ModifArticle from '@/components/ModifArticle.vue'
// import PostBlog from '@/components/PostBlog.vue'
import { ref } from 'vue';

export default {
  name: 'Admin',
  components: {
    CreateArticle, 
    // PostBlog,
    ModifArticle
  },
  setup() {
    let articles = ref([]);

    const saveBlog = function(data) {
      console.log("Admin |saveBlog() | data", data);
      articles.value =[...articles.value, {article: data, id: Date.now() }]
      console.log("Admin |saveBlog() | articles.value", articles.value);
    }
    return {
      saveBlog,
      articles
    }
  }
}
</script>

<style scoped>

</style>