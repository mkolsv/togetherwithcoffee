<template>
    <div class="twc-container">
        <div class="twc-new-features">
            <div class="twc-new-features-content">
                <h2>More features soon</h2>
                <p class="twc-new-features__paragraph">
                    We are a small (very small) group of enthusiasts who love coffee and coding.
                    And we want to create a cozy and friendly place for our like-minded people.
                    We have a lot of ideas, but we'd love to hear your suggestions as well.
                    We will be very grateful if you share your ideas and suggestions.
                    We will be happy to implement them 🤗
                </p>

                <div class="twc-new-features__actions">
                    <Button class="twc-new-features__button--ideas" skin="outlined">
                        Share ideas
                    </Button>

                    <Button skin="primary">
                        Buy us a coffee  ☕️
                    </Button>
                </div>
            </div>

            <div class="twc-new-features__media">
                <img class="twc-new-features__image" src="../../../assets/images/home/coffee-equipment.jpeg" alt="Coffee Equipment">
            </div>
        </div>
    </div>
</template>

<script setup>
import Button from '../../shared/base/Button';
</script>

<style scoped>
.twc-new-features {
    display: flex;
    height: 432px;
    padding-bottom: 40px;
}

.twc-new-features-content {
    display: flex;
    flex: 1;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.twc-new-features__paragraph {
    max-width: 400px;
    text-align: center;
    color: var(--color-text-300);
    padding: 24px 0;
}

.twc-new-features__media {
    overflow: hidden;
    flex: 1;
}

.twc-new-features__image {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.twc-new-features__button--ideas {
    margin-right: 32px;
}
</style>
