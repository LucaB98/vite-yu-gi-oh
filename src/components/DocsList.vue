<script>
import { store } from '../data/store.js';
import DocsCard from './DocsCard.vue';
export default {
    name: 'DocsList',
    data: () => ({ store }),
    components: { DocsCard }
};
</script>

<template>
    <section id="docs-list">
        <div class="row g-4 row-cols-2 row-cols-md-3 row-cols-lg-5 mx-3 pb-4">
            <div class="col d-flex justify-content-center align-items-center" v-for="doc in store.docs" :key="doc.id">
                <DocsCard :name="doc.name" :number="doc.number" :type1="doc.type1" :image="doc.imageUrl" />
            </div>
        </div>
    </section>
</template>

<style scoped>
.docs-list {
    height: 100%;
    overflow: hidden;

}

.row {

    background-image: linear-gradient(to bottom right, #62666B 70%, white);
}
</style>