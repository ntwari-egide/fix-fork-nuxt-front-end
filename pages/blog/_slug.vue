<template>
    <div>
        <AppHeader />

        <div class="flex mt-8">
            <div class="left-content pl-12" style="width: 15%;">
                <div class="icon-action">
                    <svg id="git-pull-request-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                        <path id="Path_28" data-name="Path 28" d="M0,0H29V29H0Z" fill="none"/>
                        <path id="Path_29" data-name="Path 29" d="M18.333,5.789h2.555a2.541,2.541,0,0,1,2.555,2.526v10.32a3.828,3.828,0,1,1-2.555,0V8.316H18.333v3.789l-5.75-5.053L18.333,2ZM5.556,10.627a3.8,3.8,0,1,1,5.057-4.215,3.786,3.786,0,0,1-2.5,4.215v8.008a3.8,3.8,0,1,1-5.057,4.215,3.786,3.786,0,0,1,2.5-4.215ZM6.834,8.316A1.263,1.263,0,1,0,5.556,7.053,1.271,1.271,0,0,0,6.834,8.316Zm0,15.158A1.263,1.263,0,1,0,5.556,22.21,1.271,1.271,0,0,0,6.834,23.474Zm15.333,0a1.263,1.263,0,1,0-1.278-1.263A1.271,1.271,0,0,0,22.166,23.474Z" transform="translate(0 0)"/>
                    </svg>
                </div>
                <div class="icon-action">
                    <svg id="git-pull-request-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                        <path id="Path_28" data-name="Path 28" d="M0,0H29V29H0Z" fill="none"/>
                        <path id="Path_29" data-name="Path 29" d="M18.333,5.789h2.555a2.541,2.541,0,0,1,2.555,2.526v10.32a3.828,3.828,0,1,1-2.555,0V8.316H18.333v3.789l-5.75-5.053L18.333,2ZM5.556,10.627a3.8,3.8,0,1,1,5.057-4.215,3.786,3.786,0,0,1-2.5,4.215v8.008a3.8,3.8,0,1,1-5.057,4.215,3.786,3.786,0,0,1,2.5-4.215ZM6.834,8.316A1.263,1.263,0,1,0,5.556,7.053,1.271,1.271,0,0,0,6.834,8.316Zm0,15.158A1.263,1.263,0,1,0,5.556,22.21,1.271,1.271,0,0,0,6.834,23.474Zm15.333,0a1.263,1.263,0,1,0-1.278-1.263A1.271,1.271,0,0,0,22.166,23.474Z" transform="translate(0 0)"/>
                    </svg>
                </div>
                <div class="icon-action">
                    <svg id="git-pull-request-line" xmlns="http://www.w3.org/2000/svg" width="29" height="29" viewBox="0 0 29 29">
                        <path id="Path_28" data-name="Path 28" d="M0,0H29V29H0Z" fill="none"/>
                        <path id="Path_29" data-name="Path 29" d="M18.333,5.789h2.555a2.541,2.541,0,0,1,2.555,2.526v10.32a3.828,3.828,0,1,1-2.555,0V8.316H18.333v3.789l-5.75-5.053L18.333,2ZM5.556,10.627a3.8,3.8,0,1,1,5.057-4.215,3.786,3.786,0,0,1-2.5,4.215v8.008a3.8,3.8,0,1,1-5.057,4.215,3.786,3.786,0,0,1,2.5-4.215ZM6.834,8.316A1.263,1.263,0,1,0,5.556,7.053,1.271,1.271,0,0,0,6.834,8.316Zm0,15.158A1.263,1.263,0,1,0,5.556,22.21,1.271,1.271,0,0,0,6.834,23.474Zm15.333,0a1.263,1.263,0,1,0-1.278-1.263A1.271,1.271,0,0,0,22.166,23.474Z" transform="translate(0 0)"/>
                    </svg>
                </div>
            </div>
            <div  style="width: 70%;background: yellow;height: 100vh">
            </div>
            <div style="width: 15%;background: blue;height: 100vh">
            </div>
        </div>

        <!-- <article>
            <nuxt-content :document="article" />
        </article> -->
        <!-- <article class="p-4">

            <h1>{{ article.title }}</h1>
            <p>{{ article.description }}</p>
            <img :src="article.img" :alt="article.alt" />
            <p>Article last updated: {{ formatDate(article.updatedAt) }}</p>
            
            <nuxt-content :document="article" />

            <h1>Adding code block in markdown file</h1>
            
        </article> -->
    </div>
</template>

<script>
    import AppHeader from "../../components/AppHeader.vue";

    export default{

        components: {
            AppHeader
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

.left-content div{
    border: 1px solid #CBCBCB;
    margin-bottom: 36px;
    width: 36%;
    padding: 16px;
    border-radius: 5px;
    cursor: pointer;
}


.left-content div svg{
    height: 20px;
    width: 20px;
}
</style>