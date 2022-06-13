<template>
    <form class="twc-search__form">
        <button class="twc-button twc-search__submit-button"></button>
        <input class="twc-search" type="text" :placeholder="props.placeholder">
    </form>
</template>

<script setup>
const props = defineProps({
    placeholder: {
        type: String,
        required: false,
        default: 'City, country or coffee shop'
    }
});
</script>

<style scoped>
.twc-search__form {
    position: relative;
}

.twc-search__submit-button {
    width: 16px;
    height: 16px;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 14px;
    padding: 0;
    margin-top: auto;
    margin-bottom: auto;
    background-image: url("data:image/svg+xml,%3Csvg width='16' height='16' viewBox='0 0 16 16' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cg clip-path='url(%23clip0_17_25)'%3E%3Cpath d='M0.151386 15.1295L4.28233 11.0646C3.20057 9.8893 2.5359 8.33495 2.5359 6.62455C2.53642 2.96568 5.55012 0 9.268 0C12.9859 0 15.9996 2.96568 15.9996 6.62455C15.9996 10.2834 12.9859 13.2491 9.268 13.2491C7.66162 13.2491 6.18828 12.6935 5.03099 11.7697L0.884027 15.8507C0.681966 16.0498 0.353919 16.0498 0.151857 15.8507C-0.0506744 15.6517 -0.0506763 15.3286 0.151386 15.1295ZM9.268 12.2299C12.4137 12.2299 14.9638 9.72029 14.9638 6.62455C14.9638 3.52881 12.4137 1.01923 9.268 1.01923C6.12224 1.01923 3.57217 3.52881 3.57217 6.62455C3.57217 9.72029 6.12224 12.2299 9.268 12.2299Z' fill='black'/%3E%3C/g%3E%3Cdefs%3E%3CclipPath id='clip0_17_25'%3E%3Crect width='16' height='16' fill='white' transform='matrix(-1 0 0 1 16 0)'/%3E%3C/clipPath%3E%3C/defs%3E%3C/svg%3E%0A");
    background-repeat: no-repeat;
    cursor: pointer;
}
.twc-search {
    width: 100%;
    padding: 16px 16px 16px 40px;
    outline: none;
    border: none;
    border-radius: 4px;
    background-position-y: center;
}
</style>
