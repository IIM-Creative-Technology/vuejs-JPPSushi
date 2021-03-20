<template>
    <div>
        <p>t dans l'admin frero</p>
        <CreateArticle />
    </div>
    
</template>
<script>
// @ is an alias to /src
import CreateArticle from '@/components/CreateArticle.vue'

export default {
  name: 'Admin',
  components: {
    CreateArticle
  }
}
</script>

<style scoped>

</style>