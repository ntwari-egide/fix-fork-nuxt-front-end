<template>
    <div>
        <AppHeader />
        <div class="p-4">
            <h1 class="text-lg font-semibold text-center">Joke</h1>

            <div class="joke border my-4 p-2">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Non vitae explicabo tenetur corporis dolorem eius minima. Hic minus expedita dolorem, maiores, nemo molestias mollitia dolorum itaque facere quidem quae quis! </p>
                <p class="text-sm font-semibold mt-4 text-right">joke id: {{ $route.params.id }}</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default{}
</script>

<style>

</style>