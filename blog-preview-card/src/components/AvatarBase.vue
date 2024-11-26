<script setup>
// Props
const props = defineProps({
  img: {
    type: String,
    required: true,
  },
  name: {
    type: String,
    required: true,
  },
})
</script>
<template>
  <div class="avatar-base">
    <img :src="props.img" alt="Avatar Image" width="32" height="32" />
    <span class="text-xs-extrabold-preset">{{ props.name }}</span>
  </div>
</template>
<style lang="scss" scoped>
.avatar-base {
  display: flex;
  align-items: center;
  justify-content: start;
  gap: var(--spacing-150);
}
</style>
