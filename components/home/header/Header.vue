<template>
    <header class="twc-header">
        <img src="../../../assets/images/shared/logo.svg" alt="Together with coffee">

        <Navigation />

        <Button type="secondary">
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
    background: #FFF;
    display: flex;
    justify-content: space-between;
}
</style>
