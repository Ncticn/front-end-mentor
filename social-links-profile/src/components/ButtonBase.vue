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
  <a :href="props.href" class="button-base">
    <span class="button-base-link text-bold-presets">{{ props.label }}</span>
  </a>
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
  text-align: center;
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
