<script>
export default {
    name: "AppAside",
}
</script>

<template>
    <footer>
        <nav>

        </nav>
        <div>

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

footer {
    // @include padding;
    height: 400px;
    background-color: rgb(41, 41, 41);

    nav {
        @include padding;
        height: 300px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
    }

    div {
        @include padding;
    }

}
</style>