<template>
    <div class="article">
        <img :src="image" width="500" height="auto">
        <h3>{{ title }}</h3>
        <h4>{{ source }}</h4>
        <p>{{ date }}</p>
        <p>{{ description }}</p>
        <a :href="url" target="_blank"><p>Click here to check details</p></a>
    </div>
</template>

<script>
export default {
    name: 'Article',
    props:  ['image', 'title', 'source', 'date', 'description', 'url','id']
}
</script>

<style>
    .article {
        width: 900px;
        padding: 1rem;
        border: 1px dotted #ccc;
        margin: 1rem auto;
    }
</style>