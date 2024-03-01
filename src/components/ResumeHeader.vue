<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'ResumeHeader',
  data() {
    return {}
  }
})
</script>

<template>
  <div class="header">
    <h1 class="header-h1">Дмитрий <br />Киреев</h1>
    <p class="header-p">Frontend - разработчик</p>
  </div>
</template>

<style scoped>
.header {
  float: right;
  background-color: white;
  color: #282833;
  width: 500px;
  height: 350px;
}

.header-h1 {
  font-size: 45px;
  font-family: Gill Sans, sans-serif;
  margin-bottom: 8px;
  margin-top: 100px;
}

.header-p {
  color: #282833;
  font-size: 24px;
  margin-top: 0px;
  padding-top: 0px;
}
</style>
