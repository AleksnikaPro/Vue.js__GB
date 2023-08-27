<template>
    <header class="header center">
        <div class="header__content">
            <a href="#" class="header__logo">
                <img class="header__logo-img" src="../assets/images/logo.svg" alt="logo">
            </a>
            <Navigation :style="navigation"/>
        </div>
    </header>
</template>
<script>
import Navigation from './Navigation.vue';

export default {
    name: 'Header',

    components: {
        Navigation
    }
};
</script>

<style lang="scss" scoped>

.navigation {

    &__list {
        display: flex;
        gap: 25px;
    }
    &__link {
        color: #292F36;
        font-family: 'Jost', sans-serif;
        font-weight: 400;
        font-style: normal;
        font-size: 20px;
        line-height: 1.25;
        text-align: center;

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

    // &__list {
    //     display: flex;
    //     gap: 25px;
    // }

    // &__link {
    //     @include font-jost-regular($secondPrimaryColor, 20px, 1.25);
    //     text-align: center;

    //     &:hover {
    //         color: $firstPrimaryColor;
    //         @include transition-slow();
    //     }

    //     &:active {
    //         color: $fourthPrimaryColor;
    //         @include transition-slow();
    //     }

    //     &:focus {
    //         color: $firstPrimaryColor;
    //         @include transition-slow();
    //     }
    // }

}
</style>
