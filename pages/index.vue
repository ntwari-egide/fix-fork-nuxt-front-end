<template>
    <div>
        <div class="welcome-home-page bg-blue pl-0 p-6 mb-8">
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

            <div class="header-navbar flex items-center justify-between mt-8">
                <div class="left-content flex">
                    <nuxt-link to="/" class="active-link">Home</nuxt-link>
                    <nuxt-link to="/"  class="ml-8">About</nuxt-link>
                    <nuxt-link to="/"  class="ml-8">Issues</nuxt-link>
                    <nuxt-link to="/"  class="ml-8">Questions</nuxt-link>
                    <nuxt-link to="/"  class="ml-8">Open source projects</nuxt-link>
                </div>
                <div class="right-content flex items-center">
                    <nuxt-link to="/">Login</nuxt-link>
                    <nuxt-link to="/" class="ml-8">
                        <button class="flex subscribe-button">
                        <span>
                            <svg xmlns="http://www.w3.org/2000/svg" width="18.07" height="18.07" viewBox="0 0 18.07 18.07">
                            <path id="Icon_ionic-ios-add" data-name="Icon ionic-ios-add" d="M25.91,16.875H19.125V10.09a1.125,1.125,0,0,0-2.25,0v6.785H10.09a1.125,1.125,0,0,0,0,2.25h6.785V25.91a1.125,1.125,0,0,0,2.25,0V19.125H25.91a1.125,1.125,0,0,0,0-2.25Z" transform="translate(-8.965 -8.965)" fill="#fff"/>
                            </svg>
                            </span>
                        <span>subscribe</span>
                    </button>
                    </nuxt-link>
                </div>
            </div>

        </div>
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

        <div class="mt-24 flex posts-container">
            <div class="posts">

            </div>
            <div class="latests-news">

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


.welcome-home-page{
    height: 107vh;
    background: url('../assets/images/welcome-bg.svg');
    background-size: cover;
    background-repeat: no-repeat;
}

.welcome-home-page .logo-section{
    margin-right: 45px;
}
.welcome-home-page .logo-section img{
    width: 86px;
}

.welcome-center-content .rightcontainer{
    height: 326px;
    width: 534px;
    background: rgba(255, 255, 255, 0.185);
    margin-left: 306px;
}

.welcome-center-content{
    font-family: 'Manrope';
    margin-top: 196px;
    margin-left: 20px;
}
.welcome-center-content .leftcontent p{
    margin-top: 254px;
    transform: rotate(270deg);
    color: #ffffffdb;
    font-size: 13px;
    margin-left: 14px;
}
.welcome-center-content .centercontainer {
    margin-top: 34px;
    margin-left: 229px;
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
font-size: 15px;
    font-weight: 300;
    color: #ffffffab;
    margin-top: 63px;
    margin-left: 37px;
    border: 1px solid #ffffffab;
    padding: 14px 57px;
    border-radius: 5px;
}

.welcome-center-content .centercontainer button:hover{
    background: #ffffff4a;
    transition: ease-in-out 0.4s;
}
.header-navbar{
margin-top: 209px;
    margin-left: 211px;
    color: #ffffffc7;
    font-weight: 400;
    margin-right: 38px;
}
.header-navbar .right-content .subscribe-button{
    border: 1px solid #ffffff42;
    padding: 6px 37px;
    font-size: 13px;
    border-radius: 5px;
}

.header-navbar .right-content .subscribe-button:hover{
    background: #ffffff4a;
    transition: ease-in-out 0.4s;
}

.header-navbar .left-content a:hover{
    border-bottom: 1px solid #ffffff69;
    transition: ease-in-out 0.3s;
}
.header-navbar .left-content .active-link{
    color: #ffffff;
    border-bottom: 1px solid white;
    width: 17px;
    margin-right: 15px;
}

.header-navbar .right-content .subscribe-button svg{
    height: 19px;
    padding-top: 4px;
    margin-right: 6px;
}

.post-types-container{
margin-left: 210px;
    margin-top: 74px;
    margin-bottom: 17px;
    margin-right: 54px;
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

.posts-container{
    margin-left: 210px;
    margin-bottom: 17px;
    margin-right: 54px;
}

.posts-container .posts{
    height: 400px;
    background: blue;
    width: 106px;
}

.posts-container .latests-news{
    height: 400px;
    background: green;
}


</style>