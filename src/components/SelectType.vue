<script>
export default {
    name: 'SelectType',
    data: () => ({
        items: [
            {
                name: "Bug"
            },
            {
                name: "Dark"
            },
            {
                name: "Dragon"
            },
            {
                name: "Electric"
            },
            {
                name: "Fairy"
            },
            {
                name: "Fighting"
            },
            {
                name: "Fire"
            },
            {
                name: "Flying"
            },
            {
                name: "Ghost"
            },
            {
                name: "Grass"
            },
            {
                name: "Ground"
            },
            {
                name: "Ice"
            },
            {
                name: "Normal"
            },
            {
                name: "Poison"
            },
            {
                name: "Psychic"
            },
            {
                name: "Rock"
            },
            {
                name: "Steel"
            },
            {
                name: "Water"
            }
        ],
    })
};
</script>

<template>
    <select class="form-select type-select" aria-label="Default select example">
        <option v-for="item in items" selected>{{ item.name }}</option>

    </select>
</template>

<style scoped>
.type-select {
    width: 150px;
    height: 50px;
}
</style>