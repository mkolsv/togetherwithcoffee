<template>
    <button
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
