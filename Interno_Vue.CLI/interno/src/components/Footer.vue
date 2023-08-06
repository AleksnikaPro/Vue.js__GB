<template>
    <footer class="footer center">
        <div class="footer__content">
            <div class="footer__items">
                <div class="footer__item">
                    <a href="#" class="footer__logo">
                        <img class="footer__logo-img" src="../assets/images/logo.svg" alt="logo">
                    </a>
                    <p class="footer__item-text">It is a long established fact that a reader will
                        be distracted lookings.</p>
                    <ul class="footer__icons-box">
                        <li class="footer__icon-item">
                            <a href="#" class="footer__icon-link">
                                <img src="../assets/images/tweeter.svg" alt="tweeter icon" class="footer__social-img">
                            </a>
                        </li>
                        <li class="footer__icon-item">
                            <a href="#" class="footer__icon-link">
                                <img src="../assets/images/linkedin.svg" alt="linkedin icon">
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="footer__item">
                    <p class="footer__item-heading">Pages</p>
                    <nav class="footer__item-navigation">
                        <ul class="footer__list">
                            <li v-for="link in listOfLinks" :key="link.id" class="footer__navigation-item">
                                <a href="#" class="footer__navigation-link">{{ link.linkName }}</a>
                            </li>
                        </ul>
                    </nav>
                </div>
                <div class="footer__item">
                    <p class="footer__item-heading">Contact</p>
                    <p class="footer__contact-address">
                        55 East Birchwood Ave. Brooklyn, New York 11201
                    </p>
                    <a class="footer__contact-email" href="mailto:contact@interno.com">contact@interno.com</a>
                    <a class="footer__contact-phone" href="tel:1234567890"> (123) 456 - 7890</a>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',

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