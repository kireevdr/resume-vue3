<script lang="ts">
import PhotoImage from '@/components/ResumePhoto.vue'
import ResumeHeader from '@/components/ResumeHeader.vue'
import EducationBlock from '@/components/ResumeEducation.vue'
import ExperienceBlock from '@/components/ResumeExperience.vue'
import Contacts from '@/components/ResumeContacts.vue'
import ResumeProfile from '@/components/ResumeProfile.vue'
import ResumeSkills from '@/components/ResumeSkills.vue'
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'PhotoAvatar',
  components: {
    PhotoImage,
    ResumeHeader,
    EducationBlock,
    ExperienceBlock,
    Contacts,
    ResumeProfile,
    ResumeSkills
  }

  // name: 'Contacts',
  // components: {
  //   Contacts
  // },
  // name: 'Profile',
  // components: {
  //   Profile
  // }
})
</script>

<template>
  <resume-header />

  <!-- <div id="header">
    <h1>Дмитрий <br />Киреев</h1>
    <p id="frontend">Frontend - разработчик</p>
  </div> -->

  <resume-profile />

  <!-- <div id="profile">
    <h2>Профиль</h2>

    <p id="important">
      Важно с блеском преподносить продукт окружающим, чтобы добиться успеха. Но вместе с успехом
      возникает необходимость в увеличении работы. Работа и успех взаимосвязаны. Позвольте мне
      разобраться в мельчайших деталях, этим должен заниматься специалист.
    </p>
  </div> -->

  <ExperienceBlock />

  <!-- <div id="experience">
    <h2>Опыт</h2>

    <p id="freelance">Freelance, частная практика</p>

    <p id="organisation">
      - Организация полного цикла продажи <br />
      - Проведение маркетинговых и рекламных компаний <br />
      - Организация логистических цепочек <br />
    </p>

    <p id="freelanse">Freelance, частная практика</p>

    <p id="registration">
      - Регистрация ООО, ИП, потребительских кооперативов <br />
      - Судебная практика <br />
      - Юридическое сопровождение бизнеса <br />
    </p>

    <p id="lawer">Юрисконсульт</p>

    <p id="reg">
      - Регистрация ООО, ИП <br />
      - Судебная практика <br />
    </p>

    <p id="florium">
      2017 - Present <br />
      Florium
    </p>

    <p id="szup">
      2015-2017 <br />
      СЗЮП
    </p>

    <p id="registratorSpb">
      2014-2015 <br />
      Регистратор-СПб
    </p>
  </div> -->

  <resume-skills />

  <!-- <div id="skills">
    <h2>Навыки</h2>

    <p id="js">
      JavaScript <br />
      Основы программирования <br />
      HTML и CSS <br />
    </p>

    <p id="circle">
      <span class="bot active"></span>
      <span class="bot active"></span>
      <span class="bot active"></span>
      <span class="bot"></span>
      <br />

      <span class="bot active"></span>
      <span class="bot active"></span>
      <span class="bot active"></span>
      <span class="bot"></span>
      <br />

      <span class="bot active"></span>
      <span class="bot active"></span>
      <span class="bot active"></span>
      <span class="bot"></span>
      <br />
    </p>
  </div> -->

  <!-- <div id="myPic" onclick="clickOnDiv(this)" title="Foto" alt="Фото профиля"></div> -->

  <!-- <div class="photo">
  <img id="myPic" src="@/assets/foto.jpg" title="Foto" alt="Фото профиля"/>
  </div> -->

  <photo-image />

  <contacts />

  <!-- <div id="contacts">
    <h2>Контакты</h2>
    <p>
      Телефон <br />
      +7(921)654-65-68 <br />
    </p>

    <p>
      Email <br />
      kireevdr@bk.ru <br />
    </p>

    <p>
      Адрес <br />
      г. Санкт-Петербург <br />
      Южное шоссе, 55 к 3 <br />
    </p>
  </div> -->

  <EducationBlock />

  <!-- <div id="education">
    <h2>Образование</h2>
    <p>
      2003-2005 <br />
      Оператор ЭВМ <br />
      Компьютерный колледж <br />
    </p>

    <p>
      2005 - 2010 <br />
      Специалист по направлению "Юриспруденция" <br />
      ЮУрГУ <br />
    </p>

    <p>
      2010-2013 <br />
      Аспирант юридического факультета <br />
      СПбГУ <br />
    </p>
  </div> -->
</template>

<style scoped>
/* body {
  font-family: Lucida Console;
  font-size: 14px;
  width: 800px;
  height: 1290px;
  background-color: #babebf;
  margin-left: auto;
  margin-right: auto;
} */

/* p {
  color: #c3c3c7;
  padding-left: 5px;
  margin: 35px;
  line-height: 20px;
}

h1 {
  padding-left: 40px;
} */

/* #header {
  float: right;
  background-color: white;
  color: #282833;
  width: 500px;
  height: 350px;
}

#header h1 {
  font-size: 45px;
  font-family: Gill Sans, sans-serif;
  margin-bottom: 8px;
  margin-top: 100px;
}

#header #frontend {
  color: #282833;
  font-size: 24px;
  margin-top: 0px;
  padding-top: 0px;
} */

/* #profile {
  clear: right;
  float: right;
  background-color: white;
  width: 500px;
  height: 230px;
}

#profile h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  color: #282833;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #e6eef0 97.5%, #f5c03b 2.5%);
}

#profile #important {
  color: #282833;
  padding-left: 5px;
  margin: 35px;
  line-height: 20px;
} */

/* #experience {
  clear: right;
  float: right;
  background-color: white;
  width: 500px;
  height: 470px;
}

#experience h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  color: #282833;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #e6eef0 97.5%, #f5c03b 2.5%);
}

#experience #freelance {
  color: #282833;
  padding-left: 5px;
  font-weight: bold;
  float: right;
  width: 270px;
  height: 30px;
  margin-top: 35px;
  margin-left: 0px;
  margin-right: 35px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 15px;
}

#experience #organisation {
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

#experience #freelanse {
  color: #282833;
  padding-left: 5px;
  font-weight: bold;
  margin-top: 25px;
  margin-left: 0px;
  margin-right: 35px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 15px;
  clear: right;
  float: right;
  width: 270px;
  height: 30px;
}

#experience #registration {
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

#experience #lawer {
  color: #282833;
  padding-left: 5px;
  font-weight: bold;
  margin-top: 25px;
  margin-left: 0px;
  margin-right: 35px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 15px;
  clear: right;
  float: right;
  width: 270px;
  height: 22px;
}

#experience #reg {
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

#experience #florium {
  color: #282833;
  padding-left: 5px;
  margin-top: 35px;
  margin-left: 35px;
  margin-right: 0px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 12px;
  width: 220px;
  height: 135px;
}

#experience #szup {
  color: #282833;
  padding-left: 5px;
  margin-left: 35px;
  margin-right: 0px;
  margin-bottom: 0px;
  margin-top: 0px;
  line-height: 20px;
  font-size: 12px;
  width: 220px;
  height: 135px;
}

#experience #registratorSpb {
  color: #282833;
  padding-left: 5px;
  margin-left: 35px;
  margin-right: 0px;
  margin-bottom: 0px;
  margin-top: 0px;
  line-height: 20px;
  font-size: 12px;
  width: 220px;
  height: 138px;
} */

/* #skills {
  clear: right;
  float: right;
  background-color: white;
  width: 500px;
  height: 200px;
}

#skills h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  color: #282833;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #e6eef0 97.5%, #f5c03b 2.5%);
}

#skills p {
  color: #282833;
  padding-left: 5px;
  font-weight: bold;
  margin-top: 25px;
  margin-left: 35px;
  margin-right: 35px;
  margin-bottom: 0px;
  line-height: 20px;
  font-size: 15px;
}

#skills #js {
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

#skills #circle {
  margin-top: 35px;
  margin-left: 0px;
  padding-left: 10px;
  float: left;
  width: 100px;
  height: 140px;
} */

#myPic {
  width: 300px;
  height: 470px;
  background-image: url('https://sun9-59.userapi.com/impg/Uwh2zRrFDiOOs2x8HD3ByHT7hrak90M2uq39Xw/6dALXv6bSyQ.jpg?size=300x470&quality=95&sign=13075fe5c85ed2ee78b8de607a7fa5da&type=album');
}

/* #contacts {
  padding-top: 45px;
  background-color: #3b3b47;
  color: white;
  width: 300px;
  height: 325px;
}

#contacts h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  background-color: #52525c;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #52525c 96%, #f5c03b 4%);
} */

/* #education {
  padding-top: 45px;
  background-color: #282833;
  color: #797474;
  width: 300px;
  height: 365px;
}

#education h2 {
  color: #e4e4f7;
  margin: 0px;
  padding-left: 40px;
  border-top: 40px;
  background-color: #52525c;
  letter-spacing: 1px;
  line-height: 130%;
  background: linear-gradient(to left, #52525c 96%, #f5c03b 4%);
} */
/* .bot {
  height: 12px;
  width: 12px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  margin: 0px -2px;
}

.bot.active {
  background-color: #f5c03b;
} */

/* header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
} */
</style>
