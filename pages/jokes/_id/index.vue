<template>
    <div>
        <AppHeader />
        <div class="p-4">
            <h1 class="text-lg font-semibold text-right">Joke</h1>
                <div>
                    <p>Accessed id: {{ $route.params.id }}</p>
                </div>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style>

</style>
