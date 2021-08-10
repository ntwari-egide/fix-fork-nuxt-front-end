<template>
    <div>
      <AppHeader />
      <h1>Welcome to the best corny dad's jokes</h1>
    </div>
</template>

<script>
    export default{
        // setting heading
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