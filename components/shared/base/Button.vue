<template>
    <button
        class="twc-button"
        :class="buttonClasses"
        @click="$emit('click', $event)"
        type="button"
    >
        <slot />
    </button>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps({
    type: {
        type: String,
        required: true
    }
});

const buttonClasses = computed(() => `twc-button--${props.type}`);
</script>

<style scoped>
.twc-button {
    background: none;
    border: none;
    cursor: pointer;
    padding: 10px;
    border-radius: 4px;
    transition: .2s background-color ease-in, .2s color ease-in;
}

.twc-button--secondary {
    background: var(--P200);
    border: 2px solid var(--P100);
    color: var(--P100);
}

.twc-button--secondary:hover {
    background: var(--P100);
    color: var(--P200);
}
</style>
