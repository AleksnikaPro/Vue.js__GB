<template>
    <div class="project-details__intro">
        <div class="project-details__intro-content"></div>
    </div>
    <div class="project-details center">
        <div v-for="info in projectInfo" class="project-details__content">
            <h2 class="project-details__heading">{{ info.heading }}</h2>
            <div class="project-details__text-box">
                <p class="project-details__text">{{ info.firstparagraph }}</p>
                <p class="project-details__text">{{ info.secondparagraph }}</p>
            </div>
            <Slider :slider-pictures="sliderPictures"/>
        </div>
    </div>
</template>

<script>
import { mapState } from 'vuex';

import Slider from './Slider.vue'

export default {
    name: 'ProjectDetails',

    components: {
        Slider
    },
    computed: {
        ...mapState(['projectInfo', 'sliderPictures']),
    }


}
</script>

<style></style>


