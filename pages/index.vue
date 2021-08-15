<template>
    <div>
        <WelcomeHomePage />
        <div class="post-types-container grid grid-cols-4 gap-4">
            <div class="post-type">

            </div>
        </div>
    </div>
</template>

<script>
    import Navbar from "../components/NavBar.vue";
    import WelcomeHomePage from "../components/WelcomeHomePage.vue";

    export default{

        components() {
            NavBar,
            WelcomeHomePage
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

.post-types-container{
margin-left: 210px;
    margin-top: 74px;
    margin-bottom: 17px;
}

.post-types-container .post-type{
    height: 200px;
    background: red;
}

</style>