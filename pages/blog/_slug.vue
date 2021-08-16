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
    border: 1px solid #cbcbcb70;
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