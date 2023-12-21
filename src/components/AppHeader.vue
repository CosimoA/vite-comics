<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                }, {
                    text: "COMICS",
                    url: "#",
                    current: true,
                }, {
                    text: "MOOVIE",
                    url: "#",
                    current: false,
                }, {
                    text: "TV",
                    url: "#",
                    current: false,
                }, {
                    text: "GAMES",
                    url: "#",
                    current: false,
                }, {
                    text: "COLECTIBLES",
                    url: "#",
                    current: false,
                }, {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                }, {
                    text: "FANS",
                    url: "#",
                    current: false,
                }, {
                    text: "NEWS",
                    url: "#",
                    current: false,
                }, {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <!-- logo -->
        <a href="#">
            <img class="logo" src="../assets/img/dc-logo.png" alt="logo">
        </a>

        <!-- navigazione menù principale -->
        <nav>
            <ul>
                <li v-for="link in links" :class="link.current ? 'active' : ''">
                    <a :href="link.url">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

header {
    @include padding;
    height: 100px;
    @include center (space_b);


    ul {
        list-style: none;
        @include center ();

        li {
            height: 100px;
            border-bottom: 4px solid white;

            @include center (horizontal);

            a {
                display: inline-block;
                padding: 0.5rem;
                text-decoration: none;
                font-weight: 600;
                color: black;

            }
        }


    }
}
</style>
