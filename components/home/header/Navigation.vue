<template>
    <nav class="twc-nav">
        <ul class="twc-nav--list">
            <li class="twc-nav--item" v-for="n in 3">
                <a class="twc-nav--item-link" href="#">Home</a>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'Navigation'
};
</script>

<style scoped>
.twc-nav {
    display: flex;
    justify-content: center;
    flex-grow: 1;
}

.twc-nav--list {
    display: flex;
    justify-content: space-between;
    list-style-type: none;
    min-width: 400px;
}

.twc-nav--item {
    padding: 16px;
}

.twc-nav--item-link {
    text-decoration: none;
    color: var(--black);
    text-transform: uppercase;
    font-weight: 600;
}
</style>
