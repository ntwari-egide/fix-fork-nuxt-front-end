<template>
    <nuxt-link :to=" 'blog/'+post._id ">
        <div class="pointer mt-4 post-content">
            <div class="post-cover-img">
            </div>
            <div class="post-description mt-4">
                <div class="flex">
                    <nuxt-link to="/" style="border-bottom: 1px solid rgba(0, 0, 0, 0.726); color: rgba(0, 0, 0, 0.726);" class="text-sm">JAVA SCRIPT</nuxt-link>
                    <p class="ml-8 text-sm">{{dateParser(post.createdAt)}}</p>
                </div>
                <h1 class="mt-4" style="font-weight: 500;color: rgba(0, 0, 0, 0.812);">{{post.postTitle}}</h1>
                <p class="mt-4 des">{{post.postDescription}}</p>
                <button class="mt-4">Read More</button>
                <p class="font-semibold text-sm mt-4">{{12}} comments</p>
                <hr class="ml-12 mt-4" />
            </div>
        </div>
    </nuxt-link>
</template>

<script>
export default {
    name: 'PostDisplay',
    props: ['id','post'],

    methods: {
            dateParser(isoDate){
                if(isoDate !== ""){
                    let date = new Date(isoDate);
                    let year = date.getFullYear();
                    let month = date.getMonth()+1;
                    let dt = date.getDate();
                
                    if (dt < 10) {
                    dt = '0' + dt;
                    }
                    if (month < 10) {
                    month = '0' + month;
                    }
                    return year+'-' + month + '-'+dt
                }
                else{
                    return ""
                }
                
            },

            timeParser (datePassed) {
                let isoDate= datePassed
                let result = isoDate.match(/\d\d:\d\d:\d\d/);
                return result[0];
            },

            formatDate(date) {
            const options = { year: 'numeric', month: 'long', day: 'numeric' }
            return new Date(date).toLocaleDateString('en', options)
            }
    }
    
}
</script>

<style>
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

</style>