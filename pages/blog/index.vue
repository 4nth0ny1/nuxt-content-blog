<template>
  <div class="blog-container">
    <h1 class="blog-h1">blog</h1>
    <ul>
      <li v-for="article of articles" :key="article.slug">
        <NuxtLink class="article-style" :to="{ name: 'blog-slug', params: { slug: article.slug } }">
          <!-- <img :src="article.img" /> -->
          <div>
            <h2>{{ article.title }}</h2>
            <p>by {{ article.author.name }}</p>
            <p>{{ article.description }}</p>
          </div>
        </NuxtLink>
      </li>
    </ul>
  </div>
</template>

<script>
  export default {
    async asyncData({ $content, params }) {
      const articles = await $content('articles')
        .only(['title', 'description', 'img', 'slug', 'author'])
        .sortBy('createdAt', 'asc')
        .fetch()

      return {
        articles
      }
    }
  }
</script>

<style>

  .blog-container {
    max-width: 800px;
    margin: 0 auto;
  }

  .blog-h1 {
    margin-top: 10px;
    text-align: center;
  }

  li {
    list-style: none;
    border: 1px solid black;
    border-radius: 10px;
    padding: 10px;
    margin: 10px;
  }

  .article-style {
    text-decoration: none;
    color: black;
  }

</style>