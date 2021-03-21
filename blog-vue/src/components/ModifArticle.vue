<template>
  <div>
      <ul>
        <li v-for="blog in articles" :key="blog.id">{{ blog.article }}</li>
      </ul>
      {{ articles.length }} Article{{ articles.length > 1 ? "s" : "" }}
      <hr>
      <br>
    <div class="modif-cont">
      <img src="" alt="oof" />
      <div class="post">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus quam,
          recusandae laboriosam eveniet cupiditate dolores fuga repellat tempora
          soluta voluptatibus. Beatae corporis quae consectetur quasi distinctio
          earum iure ducimus asperiores!
        </p>
      </div>
      <button class="edit">Editer</button>
      <button class="bin">X</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "ModifArticle",
  props: {
    articles: {
      type: Array,
      required: true,
    },
  },
};
</script>

<style scoped>
.modif-cont {
  display: flex;
  justify-content: center;
  align-items: center;
}
.post {
  width: 50%;
}
.bin {
  background-color: lightcoral;
}
</style>