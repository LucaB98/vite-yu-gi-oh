<script>
export default {
    name: 'AppHeader',
};
</script>

<template>
    <header>
        <div class="container">
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
</style>