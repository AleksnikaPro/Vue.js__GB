<template>
    <div class="not-found center">
        <div v-for="info in notFoundInfo" class="not-found__content">
            <div class="not-found__content_right">
                <p class="not-found__title">{{ info.title }}</p>
                <p class="not-found__text">{{ info.text }}</p>
                <div class="not-found__button-box">
                    <a href="#" class="not-found__button">
                        {{ info.buttonText }}
                        <svg class="not-found__button-arrow" width="19" height="17" viewBox="0 0 19 17" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path d="M2 8.43542L15.7232 8.29857M10.6182 1.91138L17.1412 8.43436L10.4868 15.0887"
                                stroke="#CDA274" stroke-width="2" stroke-linecap="square" stroke-linejoin="round" />
                        </svg>
                    </a>
                </div>
            </div>
            <div class="not-found__content_left">
                <img class="not-found__image" :src="info.src" :alt="info.alt">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'NotFound',

    data() {
        return {
            notFoundInfo: [
                {
                    title: '404',
                    text: 'We are sorry, but the page you requested was not found',
                    buttonText: 'Back To Home',
                    src: require('@/assets/images/not_found_img.png'),
                    alt: "not-found picture"
                }
            ]
        };
    },
};
</script>

<style lang="scss" scoped></style>