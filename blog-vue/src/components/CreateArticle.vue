<template>
  <div>
    <h1>Créer une nouvelle page blog</h1>
    <div>
      <form @submit.prevent="addPost">
        <label for="Title">Titre de la page : </label>
        <input v-model="titleToSend" type="text" name="Title" />
        <br />
        <label for="metaTitle">Meta Title : </label>
        <input type="text" name="metaTitle" />
        <br />
        <label for="metaDesc">Meta Description : </label>
        <input type="text" name="metaDesc" />
        <br />
        <label for="addImg">Ajouter une image : </label>
        <input type="text" name="addImg" />
        <br />
        <label for="Post">Corps du post : </label>
        <textarea name="Post" id="" cols="80" rows="10"></textarea>
        <br />
        <button type="submit" >Envoyer</button>
      </form>
    </div>
  </div>
</template>
<script>
import { ref } from 'vue';
export default {
  name: "CreateArticle",

  setup(props, ctx) {
    let titleToSend = ref("");

    const addPost = function () {
      console.log("Form | addPost() | titleToSend.value", titleToSend.value);
      ctx.emit("add", titleToSend.value)
      titleToSend.value = '';
    };
    return {
      titleToSend,
      addPost,
    };
  },
};
</script>

<style scoped>
textarea {
  resize: none;
  padding: 5px;
}
</style>