<script lang="ts">
import { defineComponent } from 'vue'

interface Contacts {
  name: string
  value: string
  }

interface DataObject {
  contactsData: Array<Contacts>
}

export default defineComponent({
  name: 'ContactsBlock',
  data(): DataObject {
    return {
      contactsData: [
        {
          name: 'Телефон',
          value: '+7(921)654-65-68'
        },
        {
          name: 'Email',
          value: 'kireevdr@bk.ru',
          },
        {
          name: 'Адрес',
          value: 'г. Санкт-Петербург Южное шоссе, 55 к 3'
        }
      ]
    }
  }
})
</script>

<template>
  <div class="contacts">
    <h2 class="contacts-h2">Контакты</h2>
    <p v-for="(contactsItem, index) in contactsData" :key="index" class="contacts-p">
      {{ contactsItem.name }} <br>
      {{ contactsItem.value }}
    </p>
  </div>
 </template>

<style scoped>
.contacts {
  padding-top: 45px;
  background-color: #3b3b47;
  color: white;
  width: 300px;
  height: 325px;
}

.contacts-h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  background-color: #52525c;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #52525c 96%, #f5c03b 4%);
}

.contacts-p {
  color: #c3c3c7;
  padding-left: 5px;
  margin: 35px;
  line-height: 20px;
}
</style>
