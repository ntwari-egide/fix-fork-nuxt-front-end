<template>
    <div>
      <AppHeader />
      <NavBar />
      <Nuxt />
        <div>
            <h1 class="font-bold">Add a search field</h1>        

            <div class="pb-4">
                <input
                v-model="searchQuery"
                type="search"
                autocomplete="off"
                placeholder="Search Articles"
                class="p-4 border mt-4"
                />

                <h2 class="font-bold"> Results({{articles.length}}) </h2>

                <ul v-if="articles.length">
                    <li class="italic" v-for="article of articles" :key="article.slug">
                        <NuxtLink :to="{ name: 'blog-slug', params: { slug: article.slug } }">{{ article.title }}
                        </NuxtLink>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    import Navbar from "../components/NavBar.vue";

    export default{

        components() {
            NavBar
        },
        head(){
            return {
                title: "Welcome page of dad's jokes",
                meta: [{
                    hid: "description",
                    name: 'description',
                    content: 'Best place of corny jokes listing'
                }]
            }
        },
        data(){
            return {
                searchQuery: '',
                articles: []
            }
        },
        watch: {
            async searchQuery(searchQuery){
                if (!searchQuery) {
                    this.articles = []
                return
                }

                this.articles = await this.$content('articles')
                .limit(6)
                .search(searchQuery)
                .fetch()
                
            }
        }
    }
</script>

<style>

</style>