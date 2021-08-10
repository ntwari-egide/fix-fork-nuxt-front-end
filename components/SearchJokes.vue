<template>
    <div>
       <form @submit.prevent="onSubmit">
           <input type="text" v-model="text" class="form-control" placeholder="search joke ...">
            <input type="submit" value="Search Jokes">
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
