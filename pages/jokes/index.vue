<template>
    <div>
        <AppHeader />
        <div class="p-4">
            <h1 class="text-lg font-semibold text-center">Jokes</h1>

            <SearchJoke v-on:search-text="searchText"/>

            <Joke v-for="joke in jokes" :key="joke.id" :id="joke.id" :joke="joke.joke"/>
        </div>
    </div>
</template>

<script>
    import Joke from "../../components/Joke";
    import SearchJoke from "../../components/SearchJokes";

    export default{
        
        components: {
            Joke,
            SearchJoke
        },

        methods: {
            async searchText(text){
                this.jokes = [{
                        id: '2',
                        joke: 'this is the testing joke 2, Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex nihil modi molestiae iure pariatur praesentium voluptates velit cum. Error sit facilis temporibus blanditiis quaerat quo et eos cupiditate quibusdam expedita.'
                }]
            } 
        },

        // set data information
        data(){
            return {
                jokes: []
            }
        },

        // action to run when this page is reloaded
        async created(){
            const config = {
                headers: {
                    'Accept':"application/json"
                }
            }

            try {
                // const  res = await axios.get('localhost:3000/apis/jokes', config);

                this.jokes = [
                    {
                        id: '1',
                        joke: 'this is the testing joke 1,Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex nihil modi molestiae iure pariatur praesentium voluptates velit cum. Error sit facilis temporibus blanditiis quaerat quo et eos cupiditate quibusdam expedita.'
                    },
                    {
                        id: '2',
                        joke: 'this is the testing joke 2, Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex nihil modi molestiae iure pariatur praesentium voluptates velit cum. Error sit facilis temporibus blanditiis quaerat quo et eos cupiditate quibusdam expedita.'
                    },
                    {
                        id: '3',
                        joke: 'this is the testing joke 3, Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex nihil modi molestiae iure pariatur praesentium voluptates velit cum. Error sit facilis temporibus blanditiis quaerat quo et eos cupiditate quibusdam expedita.'
                    },
                    {
                        id: '4',
                        joke: 'this is the testing joke 4, Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex nihil modi molestiae iure pariatur praesentium voluptates velit cum. Error sit facilis temporibus blanditiis quaerat quo et eos cupiditate quibusdam expedita.'
                    }
                ]

            } catch (error) {
                
            }
        },

        // setting heading
        head(){
            return {
                title: "List of jokes",
                meta: [{
                    hid: "description",
                    name: 'description',
                    content: 'Best place of corny jokes listing'
                }]
            }
        }
    }
</script>

<style>

</style>