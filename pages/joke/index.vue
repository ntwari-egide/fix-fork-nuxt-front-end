<template>
    <div>
        <div class="joke">
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
