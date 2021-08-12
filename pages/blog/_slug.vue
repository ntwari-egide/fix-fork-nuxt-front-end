<template>
    <div>
        <AppHeader />
        <!-- <article>
            <nuxt-content :document="article" />
        </article> -->
        <article class="p-4">
            <h1>{{ article.title }}</h1>
            <p>{{ article.description }}</p>
            <img :src="article.img" :alt="article.alt" />
            <p>Article last updated: {{ formatDate(article.updatedAt) }}</p>
            
            <nuxt-content :document="article" />

            <h1>Adding code block in markdown file</h1>
            <h1 class="font-bold">Add a search field</h1>
            <p>The Nuxt content module gives us the possibility of searching through our articles by using the <pre>search()</pre> method.</p>        
        </article>
    </div>
</template>

<script>
    export default{

        data(){
            return {
                searchQuery: '',
                articles: []
            }
        },

        methods: {
            formatDate(date) {
            const options = { year: 'numeric', month: 'long', day: 'numeric' }
            return new Date(date).toLocaleDateString('en', options)
            }
        },
        async asyncData({ $content, params }) {
            const article = await $content('articles', params.slug).fetch()
            return { article }
        }
    }
</script>

<style>
.nuxt-content h2 {
 font-weight: bold;
 font-size: 28px;
 }
 .nuxt-content h3 {
 font-weight: bold;
 font-size: 22px;
 }
 .nuxt-content p {
 margin-bottom: 20px;
 }
</style>