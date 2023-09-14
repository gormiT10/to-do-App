<template>
  <div>
    <div class="image-container">
      <div class="image-radius">
        <head></head> <img class="profile-pic" src="public/profile_pic1.jpg" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.image-container {
  display: flex;
  justify-content: flex-end;
}

.image-radius {
  height: 10rem;
  width: 10rem;
  border-radius: 70%;
  overflow: hidden;
}
.profile-pic {
  width: 100%;
  height: auto;
}
</style>
