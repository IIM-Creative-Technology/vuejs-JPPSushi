<template>
  <div class="about">
    <h1>This is a blog pages</h1>
    <ModifArticle />
  </div>
</template>

<script>
// @ is an alias to /src
import ModifArticle from '@/components/ModifArticle.vue'

export default {
  name: 'About',
  components: {
    ModifArticle
  }
}
</script>



<style scoped>

</style>