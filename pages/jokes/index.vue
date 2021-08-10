<template>
    <div>
        <AppHeader />
        <div>jokes</div>
    </div>
</template>

<script>
    export default{

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