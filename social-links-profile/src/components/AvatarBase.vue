<script setup>
const props = defineProps({
  imgSrc: {
    type: String,
    required: true,
  },
})
</script>
<template>
  <div class="avatar-base">
    <img :src="props.imgSrc" alt="Avatar Image" class="avatar-base-img" />
  </div>
</template>
<style>
.avatar-base{
    display: inline-block;
    width: 85px;
    height: 85px;
}
.avatar-base-img{
    max-width: 100%;
    height: auto;
    object-fit: contain;
    border-radius: 100%;
}
</style>
