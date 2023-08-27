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
                    <!-- <nav class="footer__item-navigation">
                        <ul class="footer__list">
                            <li v-for="link in listOfLinks" :key="link.id" class="footer__navigation-item">
                                <a href="#" class="footer__navigation-link">{{ link.linkName }}</a>
                            </li>
                        </ul>
                    </nav> -->
                    <Navigation class="navigation"/>
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
import Navigation from './Navigation.vue';

export default {
    name: 'Footer',

    components: {
        Navigation
    }
};
</script>

<style lang="scss" scoped>
.navigation {

    &__list {
        display: flex;
        flex-direction: column;
        align-content: flex-start;
        justify-content: center;
        align-items: flex-start;
        margin: 0;

    }
    &__item {
        padding-bottom: 24px;
    }
    &__link {
        color: #4D5053;
        font-family: 'Jost', sans-serif;
        font-weight: 400;
        font-style: normal;
        font-size: 22px;
        line-height: 1.5;
        letter-spacing: 0.22;
        margin: 0;

        &:hover {
            color: #CDA274;
            transition: all 0.8s ease-out;
        }
        &:active {
            color: #4D5053;
            transition: all 0.8s ease-out;
        }
        &:focus {
            color: #CDA274;
            transition: all 0.8s ease-out;
        }
    }

}
</style>

