<template>
    <b-button
        :variant="variant"
        :size="size"
        :to="to"
        @click="onClick"
        :exact="exact"
    >
        <span
            class="button__content"
            v-if="content"
        >{{ content }}</span>
    </b-button>
</template>

<script>

export default {
    name:       'UiButton',

    props: {
        iconHref:     {
            type: String,
            required: false,
            default: '',
        },
        iconPosition: {
            type: String,
            required: false,
            default: '',
        },
        content:      {
            type: String,
            required: false,
            default: '',
        },
        size:         {
            type: String,
            required: false,
            default: '',
        },
        variant:      {
            type: String,
            required: false,
            default: 'primary',
        },
        to: {
            type: [String, Object],
            required: false,
            default: '',
        },
        exact: {
            type: Boolean,
            required: false,
            default: true,
        },
        onClick:      {
            type: Function,
            required: false,
            default:   () => [],
        },
    },
};
</script>