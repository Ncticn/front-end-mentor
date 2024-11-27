<script setup>
// Props
const props = defineProps({
    label: {
        type: String,
        required: true,
    },
    href:{
        type: String,
    }
})
</script>
<template>
    <button type="button" class="button-base">
        <a :href="props.href" class="button-base-link">{{props.label}}</a>
    </button>
</template>
<style lang="css" scoped>
.button-base{
    width: 100%;
    border: none;
    background-color: var(--color-grey-700);
    border-radius: 8px;
}
.button-base:hover{
    background-color: var(--color-green);
}
.button-base:hover .button-base-link{
    color: var(--color-grey-800);
}
.button-base-link{
    padding: 14px 16px;
    display: block;
    color: rgba(255, 255, 255, .95);
    font-size: 14px;
    font-weight: 600;
    letter-spacing: .4px;
}
</style>