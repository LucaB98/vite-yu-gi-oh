<script>
export default {
    name: 'DocsCard',
    props: {
        name: String,
        number: Number,
        type1: String,
        image: String,
    }
};
</script>

<template>
    <div class="docs-card">
        <img :src="image" :alt="name" class="img-fluid rounded-circle shadow md-3">
        <h4>{{ number }}</h4>
        <h4>{{ name }}</h4>
        <div>{{ type1 }}</div>
    </div>
</template>

<style scoped></style>