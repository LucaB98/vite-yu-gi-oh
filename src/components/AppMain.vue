<script>
import DocsList from './DocsList.vue'
export default {
    name: 'AppMain',
    components: { DocsList }
};
</script>

<template>
    <main id="main" class="container d-flex justify-content-center align-items-center">
        <DocsList />
    </main>
</template>

<style scoped>
#main {
    background-color: #DEDEDE;
    border-radius: 25px;
    height: 80vh;

}
</style>