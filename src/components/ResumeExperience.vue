<script lang="ts">
import { defineComponent } from 'vue'

interface Experience {
  position: string
  function1: string
  function2: string
  function3?: string
  date: string
  place: string
}

interface DataObject {
  ExperienceData: Array<Experience>
}

export default defineComponent({
  name: 'ExperienceBlock',
  data(): DataObject {
    return {
      ExperienceData: [
        {
          position: 'Freelance, частная практика',
          function1: '- Организация полного цикла продаж',
          function2: '- Проведение маркетинговых и рекламных компаний',
          function3: '- Организация логистических цепочек',
          date: '2017 - Present',
          place: 'Florium'
        },
        {
          position: 'Freelance, частная практика',
          function1: '- Регистрация ООО, ИП, потребительских кооперативов',
          function2: '- Судебная практика',
          function3: '- Юридическое сопровождение бизнеса',
          date: '2015-2017',
          place: 'СЗЮП'
        },
        {
          position: 'Юрисконсульт',
          function1: '- Регистрация ООО, ИП',
          function2: '- Судебная практика',
          date: '2014-2015',
          place: 'Регистратор-СПб'
        }
      ]
    }
  }
})
</script>

<template>
  <div class="experience">
    <h2 class="experience-h2">Опыт</h2>

    <p v-for="(EducationItem, index) in ExperienceData" :key="index" class="position">
    
      <span class="position-span"> 
      {{ EducationItem.function1 }} <br /> 
      {{ EducationItem.function2 }} <br /> 
      {{ EducationItem.function3 }} <br /> </span>
    </p>

    <p v-for="(EducationItem, index) in ExperienceData" :key="index" class="date-place">
      {{ EducationItem.date }} <br />
      {{ EducationItem.place }}
    </p>
  </div>
</template>

<style scoped>
.experience {
  clear: right;
  float: right;
  background-color: white;
  width: 500px;
  height: 490px;
}

.experience-h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  color: #282833;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #e6eef0 97.5%, #f5c03b 2.5%);
}

.position {
  color: #282833;
  padding-left: 5px;
  font-weight: bold;
  float: right;
  width: 270px;
  height: 110px;
  margin-top: 35px;
  margin-left: 0px;
  margin-right: 35px;
  margin-bottom: 25px;
  line-height: 20px;
  font-size: 15px;
  }

.functions {
  color: #282833;
  padding-left: 5px;
  margin-top: 0px;
  margin-left: 0px;
  margin-right: 35px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 12px;
  clear: right;
  float: right;
  width: 270px;
  height: 80px;
}

.position-span {
  color: #282833;
  padding-left: 5px;
  margin-top: 0px;
  margin-left: -5px;
  margin-right: 35px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 12px;
  font-weight: normal;
}

.date-place {
  color: #282833;
  padding-left: 5px;
  margin-top: 35px;
  margin-left: 35px;
  margin-right: 0px;
  margin-bottom: 0px;
  line-height: 25px;
  font-size: 12px;
  width: 220px;
  height: 135px;
}
</style>
