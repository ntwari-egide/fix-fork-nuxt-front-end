<template>
    <div>
        <WelcomeHomePage />
        <div class="post-types-container grid grid-cols-4 gap-4">
            <div class="cursor post-type items-center">
                <p>Java Script</p>
            </div>
            <div class="cursor post-type items-center">
                <p>Java Script</p>
            </div>
            <div class="cursor post-type items-center">
                <p>Java Script</p>
            </div>
            <div class="cursor post-type items-center">
                <p>Java Script</p>
            </div>
            <div class="cursor post-type items-center">
                <p>Java Script</p>
            </div>
            <div class="cursor post-type items-center">
                <p>Java Script</p>
            </div>
            <div class="cursor post-type items-center">
                <p>Java Script</p>
            </div>
            <div class="cursor post-type items-center">
                <p>Java Script</p>
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
    margin-right: 60px;
}

.post-types-container .post-type{
    height: 157px;
    background: linear-gradient(rgba(0, 0, 0, 0.733),rgba(0, 0, 0, 0.466)),url('../assets/images/post-type.jpg');    
    background-size: cover;
}

.post-types-container .post-type p{
    text-align: center;
    padding: 70px;
    color: #ffffffc4;
    font-family: Manrope;
    font-weight: 400;
}

</style>