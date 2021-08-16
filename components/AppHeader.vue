<template>
        <div class="header-navbar flex items-center justify-between pt-2">
                <div class="logo-section ml-4 mt-2 flex" style="font-family: Manrope;">                    
                    <p>Fix</p>
                    <span class="ml-1">&amp;</span>
                    <p class="ml-1">Fork</p>
                </div>
                <div class="left-content flex">
                    <a href="/" class="active-link">Home</a>
                    <a href="/"  class="ml-8">About</a>
                    <a href="/"  class="ml-8">Issues</a>
                    <a href="/"  class="ml-8">Questions</a>
                    <a href="/"  class="ml-8">Open source projects</a>
                </div>
                <div class="right-content flex items-center">
                    <a href="/" class="font-semibold">Sign up</a>
                    <a href="/" class="font-semibold ml-8">Login</a>
                    <a href="/" class="ml-8">
                        <button class="flex subscribe-button">
                        <span>
                            <svg xmlns="http://www.w3.org/2000/svg" width="18.07" height="18.07" viewBox="0 0 18.07 18.07">
                            <path id="Icon_ionic-ios-add" data-name="Icon ionic-ios-add" d="M25.91,16.875H19.125V10.09a1.125,1.125,0,0,0-2.25,0v6.785H10.09a1.125,1.125,0,0,0,0,2.25h6.785V25.91a1.125,1.125,0,0,0,2.25,0V19.125H25.91a1.125,1.125,0,0,0,0-2.25Z" transform="translate(-8.965 -8.965)" fill="#fff"/>
                            </svg>
                            </span>
                        <span style="margin-top: 1px;">subscribe</span>
                    </button>
                    </a>
                </div>
            </div>
</template>

<script>
    export default{}
</script>

<style>
.header-navbar{
    color: black;
    font-weight: 400;
    margin-right: 38px;
    font-family: Manrope;
    font-size: 14px;
    position: sticky;
    top: 0px;
    background: #ffffffd6;
    height: 10vh;
    width: 100%;
    padding-right: 29px;
    z-index: 5;
}
.header-navbar .right-content .subscribe-button{
    padding: 7px 34px;
    font-size: 13px;
    border-radius: 5px;
    background: #121CFF;
    color: white;
}

.logo-section{
    font-family: 'Georama' !important;
}

.logo-section p{
    font-size: 23px;
    font-weight: 500;
    color: #121CFF;
}

.logo-section span{
    background: black;
    color: white;
    height: 22px;
    width: 21px;
    text-align: center;
    margin-top: 7px;
    border-radius: 100%;
}

.header-navbar .right-content .subscribe-button:hover{
    background: #0400fab6;
    transition: ease-in-out 0.4s;
}

.header-navbar .left-content a:hover{
    border-bottom: 1px solid #ffffff69;
    transition: ease-in-out 0.3s;
}
.header-navbar .left-content .active-link{
    color: black;
    border-bottom: 1px solid white;
    width: 17px;
    margin-right: 15px;
}

.header-navbar .right-content .subscribe-button svg{
    height: 19px;
    padding-top: 4px;
    margin-right: 6px;
}
</style>