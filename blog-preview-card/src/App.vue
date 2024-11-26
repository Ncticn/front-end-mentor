<script setup>
import CardBlogPreview from './components/CardBlogPreview.vue'
import AttributionFEMentor from './components/AttributionFEMentor.vue'
</script>
<template>
  <main>
    <CardBlogPreview
      :tag-value="'Learning'"
      :published="'Published 21 Dec 2023'"
      :title="'HTML & CSS foundations'"
      :description="'These languages are the backbone of every website, defining structure, content, and presentation.'"
      :avatar-img="'src/assets/img/image-avatar.webp'"
      :avatar-name="'Greg Hooper'"
    />
  </main>
  <footer>
    <AttributionFEMentor />
  </footer>
</template>
