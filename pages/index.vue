<template>
    <div>
        <div class="welcome-home-page bg-blue pl-0 p-6">
            <!-- <NavBar /> -->
            <div class="logo-section flex items-center justify-between">
                <img class="ml-6" src="../assets/images/logo1.svg" alt="">

                <button class="cursor">
                    <svg
                        class="h-8 w-8 fill-current text-black"
                        fill="none" stroke-linecap="round" 
                        stroke-linejoin="round" stroke-width="2" 
                        viewBox="0 0 24 24" stroke="white">
                        <path d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>

            <div class="flex welcome-center-content mt-24">
                <div class="leftcontent">
                    <p>creative digital blog</p>
                </div>
                <div class="centercontainer mt-6 ml-32">
                    <h1>Time to Get Your Code <br />Clean and in Order.</h1>
                    <h4>The longer it takes for a bug <br />to surface, the harder it is to find.</h4>
                    <button class="mt-4">Read more</button>
                </div>
                <div class="rightcontainer ml-16">

                </div>
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

.welcome-home-page{
    height: 100vh;
    background: url('../assets/images/welcome-bg.svg');
    background-size: cover;
    background-repeat: no-repeat;
}

.welcome-home-page .logo-section img{
    width: 86px;
}

.welcome-center-content .rightcontainer{
height: 326px;
    width: 518px;
    background: rgba(255, 255, 255, 0.185);
}

.welcome-center-content{
    font-family: 'Manrope';
}
.welcome-center-content .leftcontent p{
    margin-top: 254px;
    transform: rotate(270deg);
    color: #ffffffdb;
    font-size: 13px;
    margin-left: 14px;
}

.welcome-center-content .centercontainer h1{
    font-size: 27px;
    font-weight: 700;
    color: white;
    margin-top: 24px;
margin-left: 37px;}

.welcome-center-content .centercontainer h4{
    font-size: 19px;
    font-weight: 300;
    color: #ffffffab;
    margin-top: 24px;
    margin-left: 37px;
}

.welcome-center-content .centercontainer button{
font-size: 13px;
    font-weight: 300;
    color: #ffffffab;
    margin-top: 71px;
    margin-left: 37px;
    border: 1px solid #ffffffab;
    padding: 10px 60px;
    border-radius: 5px;
}

</style>