<script>
export default {
    name: "AppFooter",
    data() {
        return {
            navLinks: [
                {
                    title: "CHARACTERS",
                    href: "/characters",
                    active: false
                },
                {
                    title: "COMICS",
                    href: "/comics",
                    active: true
                },
                {
                    title: "MOVIES",
                    href: "/movies",
                    active: false
                },
                {
                    title: "TV",
                    href: "/tv",
                    active: false
                },
                {
                    title: "GAMES",
                    href: "/games",
                    active: false
                },
                {
                    title: "COLLECTIBLES",
                    href: "/collectibles",
                    active: false
                },
                {
                    title: "VIDEOS",
                    href: "/videos",
                    active: false
                },
                {
                    title: "FANS",
                    href: "/fans",
                    active: false
                },
                {
                    title: "NEWS",
                    href: "/news",
                    active: false
                },
                {
                    title: "SHOP",
                    href: "/shop",
                    active: false
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <!-- CONTAINER -->
        <div class="container">
            <!-- LOGO -->
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <!-- /LOGO -->

            <!-- NAVIGATION -->
            <nav class="nav-header">
                <ul>
                    <li v-for="(link, index) in navLinks" :key="index" :class="{ 'active': link.active }">
                        <a :href="link.href">
                            {{ link.title }}
                        </a>
                    </li>
                </ul>
            </nav>
            <!-- /NAVIGATION -->
        </div>
        <!-- /CONTAINER -->
    </header>
</template>

<style>
.logo img {
    width: 70%;
}

header .container {
    padding: 1em;

    display: flex;
    justify-content: space-between;
}

header ul {
    display: flex;
}

header ul li {
    margin-left: 1.2em;

    display: flex;
}

header .nav-header {
    display: flex;
    align-items: center;
}
</style>