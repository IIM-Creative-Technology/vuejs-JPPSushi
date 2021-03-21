<template>
    <div>
        <h1>Ceci est un article</h1>
        <div>
            <div class="post-header">
                <img src="" alt="image-pas-la">
                <p>ceci est une image</p>
            </div>
            <div class="post-txt">
                <p class="txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum fugit temporibus nesciunt omnis blanditiis voluptatem veritatis, sed, molestiae molestias cumque est odio pariatur quam fugiat deserunt recusandae necessitatibus, ipsam dolorem? Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo quidem quisquam molestiae quis dolorum, nisi quas minus nulla, fugit, adipisci ratione aliquam id incidunt minima voluptatum libero neque voluptatem veritatis.</p>
            </div>
            
        </div>

        
    </div>
</template>
<script>
export default{
    name: 'PostBlog',
}
</script>

<style scoped>
.txt{
    width: 70%;
}
.post-txt{
    display: flex;
    justify-content: center;
}
</style>