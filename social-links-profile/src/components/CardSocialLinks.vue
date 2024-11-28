<script setup>
import AvatarBase from './AvatarBase.vue'
import ButtonBase from './ButtonBase.vue'
</script>
<template>
  <div class="social-links-card">
    <div class="social-links-card-wrapper">
      <div class="social-links-card-profile-avatar">
        <AvatarBase img-src="src/assets/img/avatar-jessica.jpeg" />
      </div>

      <div class="social-links-card-profile-titles">
        <h1 class="title-presets">Jessica Randall</h1>
        <h3 class="subtitle-presets">London, United Kingdom</h3>
      </div>

      <p class="text-presets">"Front-end developer and avid reader."</p>

      <div class="social-links-card-buttons">
        <ButtonBase :label="'GitHub'" href="'#'" />
        <ButtonBase :label="'Frontend Mentor'" href="'#'" />
        <ButtonBase :label="'LinkedIn'" href="'#'" />
        <ButtonBase :label="'Twitter'" href="'#'" />
        <ButtonBase :label="'Instagram'" href="'#'" />
      </div>
    </div>
  </div>
</template>
<style lang="css" scoped>
.social-links-card {
  width: 100%;
  max-width: 384px;
  background-color: var(--color-grey-800);
  border-radius: 0.75rem;
}

.social-links-card-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: start;
  gap: 24px;
  padding: 2.5rem;
}

.social-links-card-profile-avatar {
  width: 88px;
  height: 88px;
}

.social-links-card-profile-titles {
  text-align: center;
}

.social-links-card-buttons {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 16px;
}
@media screen and (max-width: 768px) {
  .social-links-card-wrapper {
    padding: 1.5rem;
  }
}
</style>
