<template>
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
</template>
<script>
export default {
    
}
</script>

<style>


</style>