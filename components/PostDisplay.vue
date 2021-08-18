<template>
    <div class="pointer mt-4 post-content">
        <p>id: {{id}}</p>
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
</template>

<script>
export default {
    name: 'PostDisplay',
    props: ['id']
    
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