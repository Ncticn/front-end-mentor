<script setup></script>
<template>
  <div>
    <div class="qr-code-card">
      <div class="qr-code-card-wrapper">
        <img src="../assets/img/image-qr-code.png" class="qr-code-card-img" alt="QR Code Image" />
        <div class="qr-code-card-content">
          <h3 class="title-preset">Improve your front-end skills by building projects</h3>
          <p class="text-preset">
            Scan the QR code to visit Frontend Mentor and take your coding skills to the next level
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.qr-code-card {
  width: 320px;
  height: 499px;
  background-color: var(--color-white);
  border-radius: 20px;
  padding: var(--spacing-200) var(--spacing-200) var(--spacing-500) var(--spacing-200);
}
.qr-code-card-wrapper {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: center;
  gap: var(--spacing-300);
}
.qr-code-card-img {
  max-width: 100%;
  height: auto;
  object-fit: contain;
  border-radius: 10px;
}
.qr-code-card-content {
  padding: 0 var(--spacing-200);
}
</style>
