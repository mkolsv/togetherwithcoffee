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
    padding: 12px;
    transition: .1s background-color ease-in, .1s color ease-in;
}

.twc-button--outlined {
    background-color: var(--color-background-200);
    border: 2px solid var(--color-border-100);
    color: var(--color-text-100);
}

.twc-button--outlined:hover {
    background-color: var(--color-background-100);
    color: var(--color-text-200);
}
</style>
