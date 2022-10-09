<template>
    <NuxtLink to="#">
        <div class="twc-shop-preview">
            <img
                class="twc-shop-preview__image"
                :src="props.shop.cover"
                :alt="props.shop.name"
            >

            <div class="twc-shop-preview__content">
                <h3 class="twc-shop-preview__name">
                    {{ props.shop.name }}
                </h3>

                <span class="twc-shop-preview__separator" />

                <h4 class="twc-shop-preview__location">
                    {{ props.shop.city }}
                </h4>
            </div>
        </div>
    </NuxtLink>
</template>

<script setup>
const props = defineProps({
    shop: {
        type: Object,
        required: true
    }
});
</script>

<style scoped>
.twc-shop-preview {
    position: relative;
    width: 400px;
    height: 400px;
    overflow: hidden;
}

.twc-shop-preview:hover .twc-shop-preview__image {
    transform: scale(1.1);
    filter: brightness(.75);
}

.twc-shop-preview:hover .twc-shop-preview__separator {
    width: 192px;
}

.twc-shop-preview__image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: brightness(.6);
    transition: .2s all;
}

.twc-shop-preview__content {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    color: var(--color-text-200);
    text-align: center;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
}

.twc-shop-preview__name {
    font-weight: 600;
    font-size: 24px;
}

.twc-shop-preview__location {
    font-weight: 700;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 2px;
}

.twc-shop-preview__separator {
    display: block;
    width: 104px;
    height: 2px;
    background-color: var(--color-background-200);
    transition: .2s width;
    will-change: width;
}
</style>
