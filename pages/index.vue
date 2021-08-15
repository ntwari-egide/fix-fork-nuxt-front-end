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

        <div class="mt-24 flex posts-container">
            <div class="posts">
                <div class="pointer mt-4 post-content">
                    <div class="post-cover-img">
                    </div>
                    <div class="post-description mt-4">
                        <div class="flex">
                            <nuxt-link to="/" style="border-bottom: 1px solid rgba(0, 0, 0, 0.726); color: rgba(0, 0, 0, 0.726);" class="text-sm">JAVA SCRIPT</nuxt-link>
                            <p class="ml-8 text-sm">8-June-2021</p>
                        </div>
                        <h1 class="mt-4" style="font-weight: 500;color: rgba(0, 0, 0, 0.812);">SOLVING DOCKER FILE IN GITHUB - JAVASCRIPT</h1>
                        <p class="mt-4 des">Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam numquam, fugiat similique dolorum hic qui assumenda facilis odio voluptatem nostrum, deleniti minima reprehenderit.</p>
                        <button class="mt-4">Read More</button>
                        <p class="font-semibold text-sm mt-4">20 comments</p>
                        <hr class="ml-12 mt-4" />
                    </div>
                </div>
                
                <div class="pointer mt-4 post-content">
                    <div class="post-cover-img">
                    </div>
                    <div class="post-description mt-4">
                        <div class="flex">
                            <nuxt-link to="/" style="border-bottom: 1px solid rgba(0, 0, 0, 0.726); color: rgba(0, 0, 0, 0.726);" class="text-sm">JAVA SCRIPT</nuxt-link>
                            <p class="ml-8 text-sm">8-June-2021</p>
                        </div>
                        <h1 class="mt-4" style="font-weight: 500;color: rgba(0, 0, 0, 0.812);">SOLVING DOCKER FILE IN GITHUB - JAVASCRIPT</h1>
                        <p class="mt-4 des">Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam numquam, fugiat similique dolorum hic qui assumenda facilis odio voluptatem nostrum, deleniti minima reprehenderit.</p>
                        <button class="mt-4">Read More</button>
                        <p class="font-semibold text-sm mt-4">20 comments</p>
                        <hr class="ml-12 mt-4" />
                    </div>
                </div>
            </div>
            <div class="latests-news mt-4">
                <div class="opensource p-4">
                    <div class="">
                        <p style="color: #ffffffbf">Open source project</p>
                    </div>
                </div>
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
                title: "Fix&Fork: Welcome page of dad's jokes",
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
    padding: 9px 37px;
    font-size: 17px;
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
    height: 21px;
    padding-top: 8px;
    margin-right: 7px;
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
    font-family: Manrope;
}

.posts-container .posts{
    width: 57%;
}

.posts-container .latests-news{
    width: 40%;
    margin-left: 50px;
}

.posts-container .posts .post-content .post-cover-img{
    background: url("../assets/images/post-background.jpg");
    height: 324px;
    background-size: cover;
}

.posts-container .post-description .des{
    color: #000000cf;
    line-height: 29px;
    font-size: 15px;
}

.posts-container .post-description button{
    border-bottom: 1px solid #0000009e;
    color: #0000009e;
    font-weight: 400;
}


.posts-container .latests-news .opensource{
    height: 289px;
    background: linear-gradient(rgba(0, 0, 0, 0.733),rgba(0, 0, 0, 0.466)),url('../assets/images/post-type.jpg');    
    background-size: cover;
    border-radius: 15px;
}

</style>