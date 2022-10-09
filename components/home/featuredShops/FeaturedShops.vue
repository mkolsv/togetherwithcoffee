<template>
    <div class="twc-featured-shops twc-container">
        <h2>Explore coffee shops around the world</h2>
        <p class="twc-subheading">
            Find ideal coffee shops for you
        </p>

        <div class="twc-featured-shops__grid">
            <ShopPreview
                v-for="shop in shops"
                :key="shop.id"
                :shop="shop"
            />
        </div>
    </div>
</template>

<script setup>
import { ShopPreview } from '../../shared';

const shops = [
    {
        id: 1,
        name: 'The Barn',
        city: 'Berlin',
        country: 'Germany',
        cover: '../../assets/images/home/featured-1.jpeg'
    },

    {
        id: 2,
        name: 'Blur Coffee',
        city: 'Kyiv',
        country: 'Ukraine',
        cover: '../../assets/images/home/featured-2.jpeg'
    },

    {
        id: 3,
        name: 'Foundation Coffee Roasters',
        city: 'Odesa',
        country: 'Ukraine',
        cover: '../../assets/images/home/featured-3.jpeg'
    }
];
</script>

<style scoped>
.twc-featured-shops {
    padding-top: 40px;
    padding-bottom: 40px;
}

.twc-featured-shops__grid {
    display: flex;
    justify-content: space-between;
    padding-top: 32px;
}
</style>
