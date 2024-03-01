<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent ({
  name: 'ResumeSkills',
  data() {
    return {
      
    }
  }
})
</script>

<template>
<div class="skills">
    <h2 class="h2">Навыки</h2>

    <p class="js">
      JavaScript <br />
      Основы программирования <br />
      HTML и CSS <br />
      Git <br />
		  Vue.js 3 <br />
    </p>

    <p class="circle">
      <span class="bot-active"></span>
      <span class="bot-active"></span>
      <span class="bot-active"></span>
      <span class="bot"></span>
      <br />

      <span class="bot-active"></span>
      <span class="bot-active"></span>
      <span class="bot-active"></span>
      <span class="bot"></span>
      <br />

      <span class="bot-active"></span>
      <span class="bot-active"></span>
      <span class="bot-active"></span>
      <span class="bot"></span>
      <br />

      <span class="bot-active"></span>
		  <span class="bot-active"></span>
		  <span class="bot-active"></span>
		  <span class="bot"></span>
		  <br />

		  <span class="bot-active"></span>
		  <span class="bot-active"></span>
		  <span class="bot"></span>
		  <span class="bot"></span>
		  <br />
    </p>
  </div>
</template>

<style scoped>
.skills {
  clear: right;
  float: right;
  background-color: white;
  width: 500px;
  height: 180px;
}

.h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  color: #282833;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #e6eef0 97.5%, #f5c03b 2.5%);
}

.js {
  color: #282833;
  padding-left: 5px;
  font-weight: bold;
  float: left;
  width: 220px;
  height: 140px;
  margin-top: 35px;
  margin-left: 35px;
  margin-right: 0px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 15px;
}

.circle {
  margin-top: 35px;
  margin-left: 0px;
  padding-left: 10px;
  margin-bottom: 20px;
  line-height: 2;
  
  float: left;
  width: 100px;
  height: 160px;
}

.bot {
  height: 12px;
  width: 12px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  margin: 4px 3px;
}

.bot-active {
  background-color: #f5c03b;
  border-radius: 50%;
  display: inline-block;
  margin: 4px 3px;
  height: 12px;
  width: 12px;
}
</style>