<script>
import SelectType from './SelectType.vue';
export default {
    name: 'AppHeader',
    components: { SelectType }
};
</script>

<template>
    <header>
        <div class="container d-flex justify-content-between align-items-center">
            <ul class="my-3">
                <li>
                    <div class="blue m-2"></div>
                </li>
                <li>
                    <div class="cube-small red m-2"></div>
                </li>
                <li>
                    <div class="cube-small yellow m-2"></div>
                </li>
                <li>
                    <div class="cube-small green m-2"></div>
                </li>
            </ul>
            <SelectType />
            <div>
                <img src="../assets/img/logo-2.png" alt="" class="img-fluid logo">
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
ul {
    list-style-type: none;
    display: flex;
}

.blue {
    height: 100px;
    width: 100px;
    background-image: linear-gradient(to bottom right, white, blue);
    border: 5px solid white;
    border-radius: 50%;
}

.cube-small {
    height: 50px;
    width: 50px;
    border: 3px solid white;
    border-radius: 50%;

    &.red {
        background-image: linear-gradient(to bottom right, white, red);
    }

    &.yellow {
        background-image: linear-gradient(to bottom right, white, yellow);
    }

    &.green {
        background-image: linear-gradient(to bottom right, white, green);
    }
}

.logo {
    height: 150px;
}
</style>