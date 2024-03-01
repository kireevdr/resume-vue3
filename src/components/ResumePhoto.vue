<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'PhotoImage',
  data() {
    return {
      photoUrl: '@/assets/foto.jpg'
    }
  }
})
</script>

<template>
  <div class="photo-image">
    <img class="photo-image-my" src="@/assets/foto.jpg" title="Foto" alt="Фото профиля" />
  </div>
</template>

<style scoped>
.photo-image {
  width: 300px;
  height: 470px;
}

.photo-image-my {
  width: 300px;
  height: 470px;
}
</style>
