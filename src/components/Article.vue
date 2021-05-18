<template>
    <div>
        <h1>Article Component</h1>
        <h1>Article {{title}} has {{likes}} likes.</h1>
        <h3>Published - {{ isPublished ? 'yes' : 'no'}}</h3>
        <h3>Published by {{name}}</h3>
    </div>
</template>

<script>
    export default {
        name: 'Article',
        props: {
            title: String,
            likes: Number,
            isPublished: Boolean,
        },
        inject: ['name']
    }
</script>

<style scoped>

</style>