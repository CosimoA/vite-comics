<script>
export default {
    name: "AppMain",
}
</script>

<template>
    <main>
        <h2> Content Goes Here! </h2>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

main {
    @include padding;
    height: 100px;
    background-color: black;
    @include center (horizontal);


    h2 {
        color: white;
    }
}
</style>
