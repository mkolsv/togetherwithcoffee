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

<style lang="scss" scoped>
.twc-header {
    width: 80px;
    background: #FFF;
    display: flex;
    justify-content: space-between;
}
</style>
