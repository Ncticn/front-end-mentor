<script setup>
// Props
const props = defineProps({
  label: {
    type: String,
    required: true,
  },
  href: {
    type: String,
  },
})
</script>
<template>
  <button type="button" class="button-base">
    <a :href="props.href" class="button-base-link text-bold-presets">{{ props.label }}</a>
  </button>
</template>
<style lang="css" scoped>
.button-base {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 45px;
  width: 100%;
  border: none;
  background-color: var(--color-grey-700);
  border-radius: 0.5rem;
  place-content: center;
}

.button-base:hover {
  background-color: var(--color-green);
}

.button-base:hover .button-base-link {
  color: var(--color-grey-800);
}

.button-base-link {
  display: block;
  width: 100%;
  padding: 14px 16px;
}
</style>
