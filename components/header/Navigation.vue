<template>
    <nav class="twc-nav">
        <ul class="twc-nav--list">
            <li class="twc-nav--item">
                <a class="twc-nav--item-link" href="#">
                    Home
                </a>
            </li>

            <li class="twc-nav--item">
                <a class="twc-nav--item-link" href="#">
                    Search
                </a>
            </li>

            <li class="twc-nav--item">
                <a class="twc-nav--item-link" href="#">
                    Blog
                </a>
            </li>

            <li class="twc-nav--item">
                <a class="twc-nav--item-link" href="#">
                    About Us
                </a>
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
    border: 2px solid transparent;
    transition: .2s border-color;
}

.twc-nav--item:hover {
    border-color: var(--color-border-100);
}

.twc-nav--item-link {
    display: inline-block;
    color: var(--color-text-100);
    letter-spacing: 2px;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: 800;
    padding: 8px;
}
</style>
