<template>
  <div class="page">
    <div style="margin-bottom:70px">
      <section class="relative gray-bg container">
        <div class="home-page-banner">
          <img
            v-if="this.$parent.$language.current == 'ru_RU'"
            src="../assets/images/home_logo/ru.jpg"
          >
          <img
            v-if="this.$parent.$language.current == 'en_GB'"
            src="../assets/images/home_logo/en.jpg"
          >
        </div>
        <!--<h1 class="jumble">АСМТ 2020</h1>
        <p class="title">

          <translate>
            Международная конференция «Передовые и конкурентные технологии
            производства»
          </translate>
        </p>-->
        <p class="date">
          <translate>31 мая - 2 июня 2021 г.</translate>
        </p>
        <p class="corp">
          <translate>
            Московский Государственный Технологический Университет «СТАНКИН», Москва, Россия
          </translate>
        </p>
        <!--<div v-if="is_discount">
          <p class="reg-info">
            <translate>Регистрационный взнос:</translate>
          </p>
          <p class="reg-info-text">
            <translate>До 30 июня 2020г. – скидка</translate>&nbsp;
            <strong>20%</strong>
          </p>
        </div>-->
        <div class="mouse-scroll only-screen">
          <img
            src="@/assets/images/mouse_scroll.svg"
            alt
          >
        </div>
      </section>
    </div>
    <div class="section-white">
      <section
        class="container"
        style="padding-top:85px"
      >
        <h2>
          <div class="red-text">
            <translate>Информация о</translate>
          </div>
          <div>
            <translate>конференции</translate>
          </div>
        </h2>
        <p class="text">
          <translate>
            Оргкомитет ACМТ 2020 приглашает Вас принять участие в Международной конференции «Передовые и конкурентные технологии производства», которая пройдет в Москве, Россия. Конференция станет местом встречи ученых и представителей промышленности, на котором они смогут показать последние достижения в области технологии, инновации и обсудить перспективы развития производственных технологий.
          </translate>
        </p>
        <div>
          <h4 style="margin-bottom: 12px">
            <i>
              <img
                class="calendar"
                src="@/assets/images/calendar.svg"
                alt
              >
            </i>
            <translate>СРОКИ ПРОВЕДЕНИЯ</translate>
          </h4>
          <div class="table">
            <!-- <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 1 }"
                  />
                  <translate>Предварительный проект программы</translate>
                </div>
              </div>
              <div class="date">
                <translate>15 июля 2020г.</translate>
              </div>
            </div>

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 2 }"
                  />
                  <translate>Срок подачи аннотации</translate>
                </div>
              </div>
              <div class="date">
                <translate>31 октября 2020г.</translate>
              </div>
            </div>

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 3 }"
                  />
                  <translate>Уведомление о принятии</translate>
                </div>
              </div>
              <div class="date">
                <translate>7 ноября 2020г.</translate>
              </div>
            </div> -->

            <div class="flex flex-between">
              <div class="title">
                <div style="text-decoration: line-through;">
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 0 }"
                  />
                  <translate>Подача статьи</translate>
                </div>
              </div>
              <div
                class="date"
                style="text-decoration: line-through;"
              >
                <translate>2 декабря 2020г.</translate>
              </div>
            </div>
            
            <div class="flex flex-between">
              <div class="title">
                <div style="color: #9C1022;">
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 1 }"
                  />
                  <translate>Подача статьи</translate>
                </div>
              </div>
              <div
                class="date"
                style="color: #9C1022;"
              >
                <translate>2 января 2021г.</translate>
              </div>
            </div>

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 2 }"
                  />
                  <translate>Предварительное уведомление</translate>
                </div>
              </div>
              <div class="date">
                <translate>1 февраля 2021г.</translate>
              </div>
            </div>
            

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 3 }"
                  />
                  <translate>Окончательное уведомление</translate>
                </div>
              </div>
              <div class="date">
                <translate>1 марта 2021г.</translate>
              </div>
            </div>


            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 4 }"
                  />
                  <translate>Ранняя регистрация</translate>
                </div>
              </div>
              <div class="date">
                <translate>15 марта 2021г.</translate>
              </div>
            </div>

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 5 }"
                  />
                  <translate>Окончательный анонс программы</translate>
                </div>
              </div>
              <div class="date">
                <translate>15 апреля 2021г.</translate>
              </div>
            </div>

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 6 }"
                  />
                  <translate>Выставка "Металлообработка"</translate>
                </div>
              </div>
              <div class="date">
                <translate>24 мая - 28 мая 2021 г.</translate>
              </div>
            </div>

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 7 }"
                  />
                  <translate>Программа наведения мостов</translate>
                </div>
              </div>
              <div class="date">
                <translate>29 мая - 30 мая 2021 г.</translate>
              </div>
            </div>

            <div class="flex flex-between">
              <div class="title">
                <div>
                  <div
                    class="circle"
                    :class="{ circle_filled: period === 8 }"
                  />
                  <translate>Конференция ACMT</translate>
                </div>
              </div>
              <div class="date">
                <translate>31 мая - 2 июня 2021 г.</translate>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>

    
    <div class="section-white">
      <section
        class="container"
        style="padding-top:85px"
      >
        <h2>
          <translate>Партнёры</translate>
        </h2>
        
        <Hooper
          :key="slideToShow"
          :items-to-show="slideToShow"
          :infinite-scroll="true"
          :center-mode="true"
          :wheel-control="true"
          class="partnerCarussel"
        >
          <Slide
            v-for="(partner, i) in partners"
            :key="i"
            :index="i"
          >
            <a
              :href="partner.link"
              target="_blank"
              rel="noopener"
              :title="$parent.$language.current == 'ru_RU' ?
                partner.name :
                partner.engName"
            >
              <img
                :src="$parent.$language.current == 'ru_RU' ?
                  partner.img :
                  partner.engImg"
                :alt="$parent.$language.current == 'ru_RU' ?
                  partner.name :
                  partner.engName"
              >
            </a>
          </Slide>
        </Hooper>
      </section>
    </div>
  </div>
</template>

<script>
import RussianEngineerUnionRuImg from '../assets/images/partners/engineering_union_rus.jpg'
import RussianEngineerUnionEnImg from '../assets/images/partners/engineering_union_eng.jpg'

import {
  Hooper,
  Slide
} from 'hooper'

/* eslint-disable */
export default {
  name: "home",
  components: {
    Hooper,
    Slide
  },
  data() {
    let is_discount = new Date() < new Date("2020-06-30");
    let period = 1;
    let current_date = new Date();
    // if (current_date > new Date("2020-10-31")) period = 2;
    // if (current_date > new Date("2020-11-07")) period = 3;
    // if (current_date > new Date("2020-12-02")) period = 4;
    if (current_date > new Date("2021-02-01")) period = 2;
    if (current_date > new Date("2021-03-01")) period = 3;
    if (current_date > new Date("2021-03-15")) period = 4;
    if (current_date > new Date("2021-04-15")) period = 5;
    if (current_date > new Date("2021-05-24")) period = 6;
    if (current_date > new Date("2021-05-29")) period = 7;
    if (current_date > new Date("2021-05-31")) period = 8;
    return {
      is_discount,
      period,
      slideToShow: 3,
      partners: [
        {
          link: "https://soyuzmash.ru/",
          name: "Союз машиностроителей России",
          engName: "Russian Engineering Union",
          img: RussianEngineerUnionRuImg,
          engImg: RussianEngineerUnionEnImg
        }
      ]
    };
  },

  created () {
    window.onresize = () => {
      this.onWindowResize()
    }
    this.onWindowResize()
  },
  methods: {
    onWindowResize () {
      if(window.innerWidth < 1024) {
        this.slideToShow = 2
      }
      else {
        this.slideToShow = 3
      }
      if(window.innerWidth < 700) {
        this.slideToShow = 1
      }
    }
  }
};
</script>

<style lang="scss" scoped>

.partnerCarussel {
  outline: none;
  overflow: hidden;
  margin-bottom: 100px;
}

.home-page-banner{
  margin: 150px 0 18px 0;
  
  & > img {
    width: 100%;
  }
}

.jumble {
  text-align: center;
  font: 600 108px/125px "Gotham Pro";
  letter-spacing: 0;
  color: #1a1a1a;
  opacity: 1;
  margin-bottom: 20px;
  margin-top: 150px;
}
.title {
  text-align: center;
  font: 200 Italic 18px/22px "Gotham Pro";
  letter-spacing: 0;
  color: #1a1a1a;
  opacity: 1;
}
.date {
  text-align: center;
  font: Bold 24px/29px "Gotham Pro";
  letter-spacing: 0;
  color: #9c1022;
  opacity: 1;
}
.corp {
  text-align: center;
  font: 400 12px/14px "Gotham Pro";
  letter-spacing: 0;
  color: #1a1a1a;
  opacity: 1;
  max-width: 386px;
  margin: 0 auto 183px;
}
.reg-info {
  text-align: left;
  font: 600 14px/16px "Gotham Pro";
  letter-spacing: 0;
  color: #9c1022;
  opacity: 1;
}
.reg-info-text {
  text-align: left;
  letter-spacing: 0;
  color: #1a1a1a;
  opacity: 1;
}
.mouse-scroll {
  text-align: center;
}
.text {
  width: 664px;
  margin: 50px auto 60px 223px;
  text-align: left;
  font: 400 14px/22px "Gotham Pro";
  letter-spacing: 0;
  color: #1a1a1a;
  @media (max-width: 1024px) {
    width: auto;
    margin: 50px auto 60px 10%;
  }
}
.table {
  width: 400px;
  margin-left: 40px;
  margin-bottom: 88px;
  padding-bottom: 88px;

  @media (max-width: 600px) {
    width: auto;
    margin-left: 0;
  }

  .circle {
    display: inline-block;
    vertical-align: top;
    transform: translate(0, -0.22em);
    margin-right: 5px;
    height: 15px;
    width: 15px;
    border-radius: 50%;
    border: 1px solid #1a1a1a;
    background: transparent;
    &_filled {
      background: #1a1a1a;
    }
  }

  .title {
    text-align: left;
    font: 400 12px/14px "Gotham Pro";
    letter-spacing: 0;
    color: #1a1a1a;
    opacity: 1;
    margin-bottom: 12px;
  }

  .date {
    text-align: left;
    font: 500 12px/14px "Gotham Pro";
    letter-spacing: 0;
    color: #1a1a1a;
    opacity: 1;
  }
}

.calendar {
  width: 24px;
  height: 24px;
  margin-right: 5px;
}

.section-white {
  background: #ffffff;
}
</style>
