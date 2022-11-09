<template>
    <div class="twc-container">
        <h2>About Together With Coffee</h2>
        <p class="twc-subheading">
            What you can find in our resource
        </p>

        <div class="twc-about">
            <div class="twc-about__media">
                <img class="twc-about__image" src="../../../assets/images/home/about-us.jpeg" alt="Coffee Shops catalog">
            </div>

            <div class="twc-about-content">
                <h2>About our space</h2>
                <p class="twc-about-content__paragraph">
                    Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the
                    industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type
                    and scrambled it to make a type specimen book.
                </p>

                <Button skin="outlined">
                    Explore
                </Button>
            </div>
        </div>
    </div>
</template>

<script setup>
import { Button } from '../../shared/base';
</script>

<style scoped>
.twc-about {
    display: flex;
    height: 432px;
    padding-top: 32px;
}

.twc-about__media {
    overflow: hidden;
    flex: 1;
}

.twc-about__image {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.twc-about-content {
    display: flex;
    flex: 1;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.twc-about-content__paragraph {
    max-width: 400px;
    text-align: center;
    color: var(--color-text-300);
    padding: 24px 0;
}
</style>
