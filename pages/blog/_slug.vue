<template>
    <div>
        <AppHeader />

        <div class="flex mt-8">
            <div class="left-content pl-12" style="width: 15%;">
                <div style="position: sticky;top: 98px;">
                    <div class="icon-action">
                        <svg id="git-pull-request-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                            <path id="Path_28" data-name="Path 28" d="M0,0H29V29H0Z" fill="none"/>
                            <path id="Path_29" data-name="Path 29" d="M18.333,5.789h2.555a2.541,2.541,0,0,1,2.555,2.526v10.32a3.828,3.828,0,1,1-2.555,0V8.316H18.333v3.789l-5.75-5.053L18.333,2ZM5.556,10.627a3.8,3.8,0,1,1,5.057-4.215,3.786,3.786,0,0,1-2.5,4.215v8.008a3.8,3.8,0,1,1-5.057,4.215,3.786,3.786,0,0,1,2.5-4.215ZM6.834,8.316A1.263,1.263,0,1,0,5.556,7.053,1.271,1.271,0,0,0,6.834,8.316Zm0,15.158A1.263,1.263,0,1,0,5.556,22.21,1.271,1.271,0,0,0,6.834,23.474Zm15.333,0a1.263,1.263,0,1,0-1.278-1.263A1.271,1.271,0,0,0,22.166,23.474Z" transform="translate(0 0)"/>
                        </svg>
                    </div>
                    <div class="icon-action">
                        <svg xmlns="http://www.w3.org/2000/svg" width="36" height="27" viewBox="0 0 36 27">
                            <g id="Icon_feather-eye" data-name="Icon feather-eye" transform="translate(0 -4.5)">
                                <path id="Path_30" data-name="Path 30" d="M1.5,18S7.5,6,18,6,34.5,18,34.5,18,28.5,30,18,30,1.5,18,1.5,18Z" fill="none" stroke="#000" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                                <path id="Path_31" data-name="Path 31" d="M22.5,18A4.5,4.5,0,1,1,18,13.5,4.5,4.5,0,0,1,22.5,18Z" fill="none" stroke="#000" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"/>
                            </g>
                        </svg>
                    </div>
                    <div class="icon-action">
                        <svg xmlns="http://www.w3.org/2000/svg" width="29.25" height="28.125" viewBox="0 0 29.25 28.125">
                            <path id="Icon_ionic-ios-heart-empty" data-name="Icon ionic-ios-heart-empty" d="M24.75,3.938h-.07A8,8,0,0,0,18,7.594a8,8,0,0,0-6.68-3.656h-.07a7.949,7.949,0,0,0-7.875,7.945,17.115,17.115,0,0,0,3.361,9.33C10.969,27,18,32.063,18,32.063S25.031,27,29.264,21.213a17.115,17.115,0,0,0,3.361-9.33A7.949,7.949,0,0,0,24.75,3.938Zm2.925,16.116A53.929,53.929,0,0,1,18,29.587a54.01,54.01,0,0,1-9.675-9.541,15.169,15.169,0,0,1-2.981-8.163,5.966,5.966,0,0,1,5.92-5.97h.063a5.9,5.9,0,0,1,2.89.759,6.144,6.144,0,0,1,2.137,2,1.975,1.975,0,0,0,3.3,0,6.205,6.205,0,0,1,2.138-2,5.9,5.9,0,0,1,2.89-.759h.063a5.966,5.966,0,0,1,5.92,5.97A15.361,15.361,0,0,1,27.675,20.053Z" transform="translate(-3.375 -3.938)" fill="#3a3e3e"/>
                        </svg>
                    </div>
                    <div class="icon-action">
                        <svg id="chat-1-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                            <path id="Path_32" data-name="Path 32" d="M0,0H29V29H0Z" fill="none"/>
                            <path id="Path_33" data-name="Path 33" d="M12,3h5a10.051,10.051,0,0,1,0,20.1v4.4C10.75,24.987,2,21.218,2,13.051A10.026,10.026,0,0,1,12,3Zm2.5,17.59H17A7.539,7.539,0,0,0,17,5.513H12a7.519,7.519,0,0,0-7.5,7.538c0,4.536,3.077,7.5,10,10.654Z" transform="translate(0 0)"/>
                        </svg>
                    </div>
                    <div class="icon-action">
                        <svg xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                            <path id="Icon_simple-github" data-name="Icon simple-github" d="M14.5.445A14.686,14.686,0,0,0,0,15.314,14.837,14.837,0,0,0,9.914,29.42c.725.14.991-.32.991-.715,0-.353-.012-1.289-.018-2.528C6.854,27.074,6,24.183,6,24.183A3.916,3.916,0,0,0,4.39,22.008c-1.313-.922.1-.9.1-.9a3.05,3.05,0,0,1,2.221,1.531,3.047,3.047,0,0,0,4.223,1.237,3.2,3.2,0,0,1,.918-1.989c-3.22-.372-6.6-1.65-6.6-7.347a5.817,5.817,0,0,1,1.492-3.99,5.411,5.411,0,0,1,.127-3.935s1.214-.4,3.988,1.524a13.344,13.344,0,0,1,7.25,0c2.755-1.923,3.969-1.524,3.969-1.524a5.561,5.561,0,0,1,.145,3.935,5.842,5.842,0,0,1,1.486,3.99c0,5.712-3.389,6.969-6.616,7.335a3.608,3.608,0,0,1,.979,2.751c0,1.99-.018,3.588-.018,4.071,0,.39.254.855,1,.706A14.786,14.786,0,0,0,29,15.314,14.688,14.688,0,0,0,14.5.445" transform="translate(0 -0.445)"/>
                        </svg>
                    </div>
                </div>
            </div>

            <!-- MAIN POST SECTION -->

            <div class="blog-content mb-32"  style="width: 70%;">
                <div class="cover-img">                    
                </div>
                <h1 class="blog-title">SOLVING DOCKER FILE IN GITHUB - JAVASCRIPT</h1>
                <article>
                    <nuxt-content :document="article" />
                </article>

                <!-- comments section -->
                <div class="comment-section mt-24">
                    <div class="comment-container">
                        <h1 style="color: #041121">Comments (3)</h1>
                        <div class="flex mt-4">
                            <div class="avatar mt-8 text-white bg-yellow-500 rounded-full" style="width: 40px;height: 40px;text-align: center;padding: 10px;">
                                <p class="text-sm">AC</p>
                            </div>
                            <div class="comment  w-2/4 ml-8" >
                                <p class="commented-by text-sm  font-medium" style="color: #041121;font-size: 13px;">Anonymous contributor</p>
                                <p class="time" style="color: #73A7CC;font-size: 11px;">3hrs ago</p>
                                <p class="content" style="color: #041121e8;font-weight: 400;font-size: 13px;line-height: 23px;border-bottom: 2px solid #04112121;padding-bottom: 17px;">It will benefit you in your future career as well. It hight take a lot of practice to see improvement, but don’t give up.</p>

                                <div class="comment-reaction flex">
                                    <div class="reaction flex">
                                        <svg class="mt-4" style="width: 21px;height: 21px;" xmlns="http://www.w3.org/2000/svg" width="29.25" height="28.125" viewBox="0 0 29.25 28.125">
                                            <path id="Icon_ionic-ios-heart" data-name="Icon ionic-ios-heart" d="M24.75,3.938h-.07A8,8,0,0,0,18,7.594a8,8,0,0,0-6.68-3.656h-.07a7.949,7.949,0,0,0-7.875,7.945,17.115,17.115,0,0,0,3.361,9.33C10.969,27,18,32.063,18,32.063S25.031,27,29.264,21.213a17.115,17.115,0,0,0,3.361-9.33A7.949,7.949,0,0,0,24.75,3.938Z" transform="translate(-3.375 -3.938)" fill="#ed5622"/>
                                        </svg>
                                        <p class="ml-2 mt-3" style="font-size: 13px;color: #041121;">23 likes</p>
                                    </div>
                                    <div class="reaction flex ml-4">
                                        
                                        <svg class="mt-4" style="width: 21px;height: 21px;" id="chat-1-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                                            <path id="Path_26" data-name="Path 26" d="M0,0H29V29H0Z" fill="none"/>
                                            <path id="Path_27" data-name="Path 27" d="M12,3h5a10.051,10.051,0,0,1,0,20.1v4.4C10.75,24.987,2,21.218,2,13.051A10.026,10.026,0,0,1,12,3Zm2.5,17.59H17A7.539,7.539,0,0,0,17,5.513H12a7.519,7.519,0,0,0-7.5,7.538c0,4.536,3.077,7.5,10,10.654Z" transform="translate(0 0)" fill="#3a3e3e"/>
                                        </svg>

                                        <p class="ml-2 mt-3" style="font-size: 13px;color: #041121;">2 replies</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- comment replies -->

                <div class="flex mt-4 ml-16">
                    <div class="avatar mt-8 text-white bg-yellow-500 rounded-full" style="width: 40px;height: 40px;text-align: center;padding: 10px;">
                                <p class="text-sm">AC</p>
                    </div>
                    <div class="comment  w-2/4 ml-8" >
                            <p class="commented-by text-sm  font-medium" style="color: #041121;font-size: 13px;">Anonymous contributor</p>
                            <p class="time" style="color: #73A7CC;font-size: 11px;">3hrs ago</p>
                            <p class="content" style="color: #041121e8;font-weight: 400;font-size: 13px;line-height: 23px;border-bottom: 2px solid #04112121;padding-bottom: 17px;">It will benefit you in your future career as well. It hight take a lot of practice to see improvement, but don’t give up.</p>

                            <div class="comment-reaction flex">
                                <div class="reaction flex">
                                    <svg class="mt-4" style="width: 21px;height: 21px;" xmlns="http://www.w3.org/2000/svg" width="29.25" height="28.125" viewBox="0 0 29.25 28.125">
                                        <path id="Icon_ionic-ios-heart" data-name="Icon ionic-ios-heart" d="M24.75,3.938h-.07A8,8,0,0,0,18,7.594a8,8,0,0,0-6.68-3.656h-.07a7.949,7.949,0,0,0-7.875,7.945,17.115,17.115,0,0,0,3.361,9.33C10.969,27,18,32.063,18,32.063S25.031,27,29.264,21.213a17.115,17.115,0,0,0,3.361-9.33A7.949,7.949,0,0,0,24.75,3.938Z" transform="translate(-3.375 -3.938)" fill="#ed5622"/>
                                    </svg>
                                    <p class="ml-2 mt-3" style="font-size: 13px;color: #041121;">23 likes</p>
                                </div>
                            </div>
                        </div>
                    </div>

                <div class="flex mt-4 ml-16">
                    <div class="avatar mt-8 text-white bg-yellow-500 rounded-full" style="width: 40px;height: 40px;text-align: center;padding: 10px;">
                                <p class="text-sm">AC</p>
                    </div>
                    <div class="comment  w-2/4 ml-8" >
                            <p class="commented-by text-sm  font-medium" style="color: #041121;font-size: 13px;">Anonymous contributor</p>
                            <p class="time" style="color: #73A7CC;font-size: 11px;">3hrs ago</p>
                            <p class="content" style="color: #041121e8;font-weight: 400;font-size: 13px;line-height: 23px;border-bottom: 2px solid #04112121;padding-bottom: 17px;">It will benefit you in your future career as well. It hight take a lot of practice to see improvement, but don’t give up.</p>

                            <div class="comment-reaction flex">
                                <div class="reaction flex">
                                    <svg class="mt-4" style="width: 21px;height: 21px;" xmlns="http://www.w3.org/2000/svg" width="29.25" height="28.125" viewBox="0 0 29.25 28.125">
                                        <path id="Icon_ionic-ios-heart" data-name="Icon ionic-ios-heart" d="M24.75,3.938h-.07A8,8,0,0,0,18,7.594a8,8,0,0,0-6.68-3.656h-.07a7.949,7.949,0,0,0-7.875,7.945,17.115,17.115,0,0,0,3.361,9.33C10.969,27,18,32.063,18,32.063S25.031,27,29.264,21.213a17.115,17.115,0,0,0,3.361-9.33A7.949,7.949,0,0,0,24.75,3.938Z" transform="translate(-3.375 -3.938)" fill="#ed5622"/>
                                    </svg>
                                    <p class="ml-2 mt-3" style="font-size: 13px;color: #041121;">23 likes</p>
                                </div>
                            </div>
                        </div>
                    </div>
                
            </div>
            <div class="right-content pl-16" style="width: 15%;">
                <div style="position: sticky;top: 98px;">
                    <div class="icon-action">
                        <svg id="slideshow-2-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                            <path id="Path_34" data-name="Path 34" d="M0,0H29V29H0Z" fill="none"/>
                            <path id="Path_35" data-name="Path 35" d="M15.75,20.75V24.5H22V27H7V24.5h6.25V20.75H4.5A1.25,1.25,0,0,1,3.25,19.5V4.5H2V2H27V4.5H25.75v15a1.25,1.25,0,0,1-1.25,1.25Zm-10-2.5h17.5V4.5H5.75ZM12,7l6.25,4.375L12,15.75Z"/>
                        </svg>
                    </div>
                    <div class="icon-action">
                        <svg id="pencil-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                            <path id="Path_36" data-name="Path 36" d="M0,0H29V29H0Z" fill="none"/>
                            <path id="Path_37" data-name="Path 37" d="M19.269,11.538,17.462,9.731,5.556,21.636v1.807H7.364L19.269,11.538Zm1.807-1.807,1.807-1.807L21.077,6.116,19.269,7.923ZM8.422,26H3V20.576L20.173,3.4a1.278,1.278,0,0,1,1.807,0L25.6,7.02a1.278,1.278,0,0,1,0,1.807L8.424,26Z" transform="translate(0 0)"/>
                        </svg>
                    </div>
                </div>
            </div>
        </div>

        <div class="mt-16">
            <Footer />
        </div>
    </div>
</template>

<script>
    import AppHeader from "../../components/AppHeader.vue";
    import Footer from "../../components/Footer.vue";

    export default{

        components: {
            AppHeader,
            Footer
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

.left-content div div{
border: 1px solid #cbcbcb70;
    margin-bottom: 36px;
    padding: 16px;
    border-radius: 5px;
    cursor: pointer;
    width: 55px;
}


.left-content div div svg,
.right-content div div svg{
    height: 20px;
    width: 20px;
}

.right-content div div{
    border: 1px solid #cbcbcb70;
    margin-bottom: 36px;
    padding: 16px;
    border-radius: 5px;
    cursor: pointer;
    width: 55px;
}

.blog-content .cover-img{
    background: url("../../assets/images/post-background.jpg");
    height: 63vh;
    background-size: cover;
    width: 100%;
}

.blog-content {
    font-family: 'Manrope';
    text-align: justify;
    font-size: 14px;
    line-height: 29px;
    z-index: 0;
}

.blog-content .blog-title{
    color: blue;
    font-weight: 500;
    font-family: Manrope;
    font-size: 25px;
    text-transform: uppercase;
    margin-top: 32px;
    text-align: center;
    margin-bottom: 10px;
}

.blog-content h1{
    font-weight: 500;
    font-size: 16px;
    margin-bottom: 16px;
    margin-top: 20px;
}

.blog-content h2{
    font-weight: 500;
    font-size: 13px;
    margin-bottom: 16px;
    margin-top: 20px;
}

.blog-content a{
    font-weight: 400;
    font-size: 13px;
    margin-bottom: 16px;
    margin-top: 20px;
    color: #7798f5;
    border-bottom: 1px solid #7798f5;
}

.blog-content a:hover{
    color: #233771;
    border-bottom: 1px solid #233771;
}

.nuxt-content-highlight {
 @apply relative;
}

.nuxt-content-highlight .filename {
 @apply absolute right-0 text-gray-600 font-light z-10 mr-2 mt-1 text-sm;
}

</style>