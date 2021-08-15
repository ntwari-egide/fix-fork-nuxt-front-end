<template>
    <div>
        <div class="welcome-home-page bg-blue">

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

.welcome-home-page{
    height: 100vh;
    background: url('../assets/images/welcome-bg.svg');
    background-size: cover;
    background-repeat: no-repeat;
}

</style>