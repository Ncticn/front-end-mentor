<script setup>
// Props
const props = defineProps({
  modelValue: {
    type: String,
    required: true,
  },
})
</script>
<template>
  <div class="tag-base">
    <span class="text-xs-extrabold-preset">
      {{ props.modelValue }}
    </span>
  </div>
</template>
<style lang="scss" scoped>
.tag-base {
  width: 82px;
  height: 29px;
  padding: var(--spacing-150) var(--spacing-50);
  background-color: var(--color-yellow);
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
