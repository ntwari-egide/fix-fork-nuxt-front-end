<template>
    <div>
        <AppHeader />
        <article>
            <nuxt-content :document="article" />
        </article>
        <article>
            <h1>{{ article.title }}</h1>
            <p>{{ article.description }}</p>
            <img :src="article.img" :alt="article.alt" />
            <p>Article last updated: {{ formatDate(article.updatedAt) }}</p>
            <nuxt-content :document="article" />
        </article>
    </div>
</template>

<script>
    export default{
        async asyncData({ $content, params }) {
            const article = await $content('articles', params.slug).fetch()
            return { article }
        }
    }
</script>

<style>

</style>