<template>
    <div class="twc-slider">
        <img class="twc-slider__image" src="../../../assets/images/home/slide-1.jpeg" alt="Coffee Shop">

        <div class="twc-slider__content twc-container">
            <h1 class="twc-slider__title">
                Discover the third wave of coffee
            </h1>

            <p class="twc-slider__subtitle">
                Let's find the best coffee shops together 😍 ☕️
            </p>

            <Search class="twc-slider__search" />
            <p class="twc-slider__search-hint">
                Try: Amsterdam or The Barn
            </p>
        </div>
    </div>
</template>

<script setup>
import Search from '../../shared/Search';
</script>

<style scoped>
.twc-slider {
    max-height: 600px;
    overflow: hidden;
    position: relative;
}

.twc-slider__image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: brightness(0.7);
}

.twc-slider__content {
    position: absolute;
    top: 120px;
    left: 0;
    right: 0;
    color: #FFF;
}

.twc-slider__title {
    max-width: 400px;
    font-size: 44px;
}

.twc-slider__subtitle {
    font-size: 20px;
    font-weight: 300;
}

.twc-slider__search {
    width: 740px;
}
</style>
