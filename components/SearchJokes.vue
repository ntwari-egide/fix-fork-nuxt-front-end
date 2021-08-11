<template>
    <div>
       <form @submit.prevent="onSubmit" class="form-control">
           <input type="text" v-model="text" class="p-2 border" placeholder="search joke ...">
            <input type="submit" class="p-2 border" value="Search Jokes">
       </form>
    </div>
</template>

<script>
export default {
    name: 'SearchJokes',
    data(){
        return {
            text : ''
        }
    },
    methods: {
        onSubmit (){
            this.$emit("search-text",this.text);
            this.text = ""
        }
    }   
}
</script>

<style>

</style>
