<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'ResumeProfile',
  data() {
    return {}
  }
})
</script>

<template>
  <div class="profile">
    <h2 class="profile-h2">Профиль</h2>

    <p class="profile-p">
      Важно с блеском преподносить продукт окружающим, чтобы добиться успеха. Но вместе с успехом
      возникает необходимость в увеличении работы. Работа и успех взаимосвязаны. Позвольте мне
      разобраться в мельчайших деталях, этим должен заниматься специалист.
    </p>
  </div>
</template>

<style scoped>
.profile {
  clear: right;
  float: right;
  background-color: white;
  width: 500px;
  height: 230px;
}

.profile-h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  color: #282833;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #e6eef0 97.5%, #f5c03b 2.5%);
}

.profile-p {
  color: #282833;
  padding-left: 5px;
  margin: 35px;
  line-height: 20px;
  text-align: justify;
  text-indent: 30px;
}
</style>
