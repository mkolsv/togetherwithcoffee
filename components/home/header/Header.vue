<template>
    <header class="twc-header twc-container">
        <img src="../../../assets/images/shared/logo.svg" alt="Together with coffee">

        <Navigation />

        <Button class="twc-header__button" type="secondary">
            Any ideas?
        </Button>
    </header>
</template>

<script setup>
import Button from '../../shared/base/Button';
import Navigation from './Navigation';
</script>

<style scoped>
.twc-header {
    height: 80px;
    background: var(--P200);
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.twc-header__button {
    font-size: 14px;
}
</style>
