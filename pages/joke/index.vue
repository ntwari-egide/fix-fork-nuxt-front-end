<template>
    <div>
        <div class="joke border my-4 p-2">
            <p>{{ joke }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Joke',
    props: ['joke','id']
}
</script>

<style>

</style>
