<template>
  <div class="page">
    <div
      class="container"
      style="margin-top: 50px; margin-bottom:100px"
    >
      <div class="flex wrap flex-between">
        <div class="col-5 col-sm-12">
          <h2 style="margin-bottom:30px">
            <div class="red-text">
              <translate>Принять</translate>
            </div>
            <div>
              <translate>Участие</translate>
            </div>
          </h2>
          <p>
            <translate>
              Авторам предлагается представить полную статью до 2 января на английском языке, примерно от 6 до 10 страниц.
            </translate>
          </p>
          <p>
            <translate>
              Статьи должны быть представлены в International Journal of Advanced Manufacturing Technology:
            </translate><br>
            <a
              href="https://www.editorialmanager.com/jamt/default.aspx"
              target="_blank"
              rel="noopener nooferrer"
            >https://www.editorialmanager.com/jamt/default.aspx</a>
          </p>
          <p>
            <translate>
              Дополнительную информацию, а также готовый шаблон слов можно найти на сайте конференции.
            </translate><br>
            <a href="https://acmt2020.stankin.ru">https://acmt2020.stankin.ru</a>
          </p>

          <div style="margin: 40px 0px;">
            <h2>
              <div class="red-text">
                <span><translate>Аэропорты</translate></span>
              </div>
              <span><translate>Москвы</translate></span>
            </h2>
            <p>
              <span><translate>Шереметьево (Москва)</translate></span> SVO/UUEE
            </p>
            <p>
              <span><translate>Домодедово (Москва)</translate></span> DME/UUDD
            </p>
            <p>
              <span><translate>Внуково (Москва)</translate></span> VKO/UUWW
            </p>
          </div>
        </div>

        <div class="col-6 col-sm-12">
          <div style="margin-bottom:50px">
            <h3 style="margin-bottom:15px">
              <div class="red-text">
                <translate>ПРАВИЛА</translate>
              </div>
              <div>
                <translate>ПУБЛИКАЦИЙ</translate>
              </div>
            </h3>
            <p>
              <translate>
                Все принятые доклады конференции будут опубликованы в изданиях, индексируемых в базах Web of Science и Scopus.
              </translate>
              <br>
              <!-- <a
                href="/docs/ACMT2020_Doc_Template.docm"
                style="font-size: 12pt; font-weight: 500;"
                download
              >
                <translate>Шаблон для статей</translate> 1
              </a><br> -->

              
              <!--Springer journals-->
              <a
                href="/docs/template_ACMT_word2.dotm"
                download
              >
                <translate>Шаблон для статей</translate>
              </a><br>

              
              <a
                href="/docs/Latex_Template.zip"
                download
              >
                <translate>Шаблон для статей</translate> (LaTeX, zip)
              </a>
            </p>
          </div>

          <div>
            <h3 style="margin-bottom:15px">
              <div class="red-text">
                <translate>РЕГИСТРАЦИОННЫЙ</translate>
              </div>
              <div>
                <translate>ВЗНОС</translate>
              </div>
            </h3>
            <p>
              <translate>Крайний срок ранней регистрации: 30 февраля 2020 г.</translate> - &nbsp;
              <strong>
                <translate>28400 руб.</translate>
              </strong>
            </p>
            <p>
              <translate>Полная регистрация</translate>&nbsp;
              <strong>
                <translate>35500 руб.</translate>
              </strong>
            </p>
          </div>

          <div style="margin: 40px 0px;">
            <h2>
              <div class="red-text">
                <span><translate>Рекомендуемые</translate></span>
              </div>
              <span><translate>отели</translate></span>
            </h2>
            <p>
              <span><translate>Гостиница "Памир"</translate></span>
            </p>
            <p>
              <span><translate>Гостиница "Тянь-Шань"</translate></span>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
/* eslint-disable */

export default {
  name: "place",
  data() {
    return {
      images: [
        require("../assets/images/gallery/Image 5.png"),
        require("../assets/images/english.png")
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.text {
  margin: 0 0 5px;
  padding: 0;
  font: 400 16px/44px "Gotham Pro";
  letter-spacing: 0;
  color: #1a1a1a;
  i {
    margin-right: 8px;
    img {
      height: 24px;
      width: 24px;
      transform: translate(0, 5px);
    }
  }
  a {
    text-decoration: none;
    color: #1a1a1a;
    cursor: pointer;
  }
}
p {
  text-align: left;
  font: 400 12px/16px "Gotham Pro";
  letter-spacing: 0;
  color: #1a1a1a;
  a {
    color: #9c1022;
  }
  strong {
    font: 600 12px/16px "Gotham Pro";
    letter-spacing: 0;
    color: #9c1022;
  }
}
</style>
