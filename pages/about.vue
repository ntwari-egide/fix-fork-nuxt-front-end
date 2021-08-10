<template>
    <div>
        <AppHeader />
        <h1>About dad's jokes</h1>
        <p>This is an app which manage dad's jokes</p>
    </div>
</template>

<script>
    export default{
        // setting heading
        head(){
            return {
                title: "About the app",
                meta: [{
                    hid: "description",
                    name: 'description',
                    content: 'Best place of corny jokes'
                }]
            }
        }
    }
</script>

<style>

</style>