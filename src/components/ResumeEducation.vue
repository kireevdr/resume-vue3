<script lang="ts">
import { defineComponent } from 'vue'

interface Education {
  date: string
  speciality: string
  place: string
}

interface DataObject {
  EducationData: Array<Education>
}

export default defineComponent({
  name: 'EducationBlock',
  data(): DataObject {
    return {
      EducationData: [
        {
          date: '2003-2005',
          speciality: 'Оператор ЭВМ',
          place: 'Компьютерный колледж'
        },
        {
          date: '2005 - 2010',
          speciality: 'Специалист по направлению "Юриспруденция"',
          place: 'ЮУрГУ'
        },
        {
          date: '2010-2013',
          speciality: 'Аспирант юридического факультета',
          place: 'СПбГУ'
        }
      ]
    }
  }
})
</script>

<template>
  <div class="education">
    <h2 class="education-h2">Образование</h2>
    <p class="education-p" v-for="(EducationItem, index) in EducationData" :key="index">
      {{ EducationItem.date }} <br />
      {{ EducationItem.speciality }} <br />
      {{ EducationItem.place }} <br />
    </p>
  </div>
</template>

<style scoped>
.education {
  padding-top: 45px;
  background-color: #282833;
  color: #797474;
  width: 300px;
  height: 365px;
 }

 .education-p {
  margin-bottom: -10px;
 }

.education-h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  background-color: #52525c;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #52525c 96%, #f5c03b 4%);
}
</style>
