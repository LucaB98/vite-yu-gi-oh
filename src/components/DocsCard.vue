<script>
import { colorMap } from '../data/colorMap';
export default {
    name: 'DocsCard',
    props: {
        name: String,
        number: Number,
        type1: String,
        image: String,
    },
    computed: {
        bgColor() {
            return colorMap[this.type1];
        }
    }
};
</script>

<template>
    <div class="docs-card d-flex justify-content-center align-items-center flex-column "
        :style="`background-color: ${bgColor}`">
        <img :src="image" :alt="name" class="img-fluid rounded-circle shadow my-3">
        <h5>{{ number }}</h5>
        <h6 class="m-0">{{ name }}</h6>
        <div class="mb-2">{{ type1 }}</div>
    </div>
</template>

<style scoped>
img {
    height: 150px;
    width: 150px;

}

.docs-card {
    height: 250px;
    width: 250px;
    border-radius: 10px;
}

h6 {
    font-weight: 900;
}

.Fire {
    background-color: #FDDFDF;
}

.Grass {
    background-color: #DEFDE0;
}

.Water {
    background-color: #DEF3FD;
}
</style>