<script setup>
// İmports
import TagBase from './TagBase.vue'
import AvatarBase from './AvatarBase.vue'

// Props
const props = defineProps({
  tagValue: {
    type: String,
    required: false,
  },
  published: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
  },
  avatarImg: {
    type: String,
    required: true,
  },
  avatarName: {
    type: String,
    required: true,
  },
})
</script>
<template>
  <div class="blog-preview-card">
    <div class="blog-preview-card-img-wrapper">
      <img
        class="blog-preview-card-img"
        src="../assets/img/illustration-article.svg"
        alt="Card Image"
      />
    </div>
    <div class="blog-preview-card-content">
      <TagBase v-if="props.tagValue" :model-value="props.tagValue" />
      <span class="text-xs-medium-preset">{{ props.published }}</span>
      <h1 class="title-preset">{{ props.title }}</h1>
      <p class="text-s-medium-preset">{{ props.description }}</p>
    </div>
    <AvatarBase :img="props.avatarImg" :name="props.avatarName" />
  </div>
</template>
<style lang="scss" scoped>
.blog-preview-card {
  max-width: 384px;
  max-height: 522px;
  padding: var(--spacing-300);
  border: 1px solid var(--color-gray-950);
  border-radius: 20px;
  background-color: var(--color-white);
  filter: drop-shadow(8px 8px 0px #000000);

  &-img-wrapper {
    margin-bottom: var(--spacing-300);
  }

  &-img {
    max-width: 100%;
    height: auto;
    object-fit: contain;
    border-radius: 10px;
  }
  &-content {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: center;
    gap: var(--spacing-150);
    margin-bottom: 24px;
  }
}
</style>
