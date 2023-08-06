<template>
    <header class="header center">
        <div class="header__content">
            <a href="#" class="header__logo">
                <img class="header__logo-img" src="../assets/images/logo.svg" alt="logo">
            </a>
            <nav class="header__navigation">
                <ul class="header__navigation-list">
                    <li v-for="link in listOfLinks" :key="link.id" class="header__navigation-item">
                        <a href="#" class="header__navigation-link"> {{ link.linkName }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script>
export default {
    name: 'Header',

    data() {
        return {
            listOfLinks: [
                { id: "home", linkName: 'Home' },
                { id: "project", linkName: 'Project' },
                { id: "blog", linkName: 'Blog' },
            ]
        };
    },
};
</script>

<style></style>
