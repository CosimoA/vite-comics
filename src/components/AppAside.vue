<script>
export default {
    name: "AppAside",
}
</script>

<template>
    <aside></aside>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

aside {
    @include padding;
    height: 150px;
    background-color: blue;
    @include center (horizontal);
}
</style>