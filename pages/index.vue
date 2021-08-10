<template>
    <div>
      <AppHeader />
      <Nuxt />
    </div>
</template>

<script>
    export default{
        head(){
            return {
                title: "Welcome page of dad's jokes",
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