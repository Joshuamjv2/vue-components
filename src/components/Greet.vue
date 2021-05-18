<template>
    <h1>Hello {{name}} a.k.a {{heroName}}</h1>
    <!-- <h3>title='Jackson' is :age='15' years old</h3> -->
</template>

<script>
    export default {
        name: 'Greet',
        props: ['name', 'heroName']
    }
</script>

<style scoped>

</style>
