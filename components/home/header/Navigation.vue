<template>
    <nav class="twc-nav">
        <ul class="twc-nav--list">
            <li class="twc-nav--item" v-for="n in 4">
                <a class="twc-nav--item-link" href="#">Home</a>
            </li>
        </ul>
    </nav>
</template>

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
    min-width: 450px;
}

.twc-nav--item {
    padding: 8px;
    border: 2px solid transparent;
    transition: .2s border-color;
}

.twc-nav--item:hover {
    border-color: var(--P100);
}

.twc-nav--item-link {
    color: var(--P100);
    letter-spacing: 2px;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: 500;
}
</style>
