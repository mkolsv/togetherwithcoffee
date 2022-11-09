<template>
    <button
        class="twc-button"
        :class="buttonClasses"
        :type="props.type"
        @click="$emit('click', $event)"
    >
        <slot />
    </button>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps({
    skin: {
        type: String,
        required: true
    },

    type: {
        type: String,
        required: false,
        default: 'button'
    }
});

const buttonClasses = computed(() => `twc-button--${props.skin}`);
</script>

<style scoped>
.twc-button {
    padding: 12px;
    font-size: 14px;
    transition: .1s background-color ease-in, .1s color ease-in;
}

.twc-button--primary {
    background-color: var(--color-background-100);
    border: 2px solid var(--color-border-100);
    color: var(--color-text-200);
}

.twc-button--primary:hover {
    background-color: var(--color-background-200);
    color: var(--color-text-100);
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
