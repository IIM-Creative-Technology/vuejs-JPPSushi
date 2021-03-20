<template>
    <div>
        <h1>Créer une nouvelle page blog</h1>
        <div>
            <div >
                <p>Titre de la page</p>
                <input type="text">
                <p>Meta Title</p>
                <input type="text">
                <p>Meta Description</p>
                <input type="text">
                <p>Ajouter une image</p>
                <input type="text">
                <p>Corps du post</p>
                <textarea name="post" id="" cols="80" rows="10"></textarea>

            </div>
            
        </div>

        
    </div>
</template>
<script>
export default{
    name: 'CreateArticle',
}
</script>

<style scoped>
textarea{
    resize: none;
    padding: 5px;
}
</style>