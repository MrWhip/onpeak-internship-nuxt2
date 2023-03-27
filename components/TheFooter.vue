<template>
  <footer>
    <div class="footer">
      <div class="footer__firstBlock">
        <div class="footer__firstBlockColumn">
          <div class="footer__firstBlockColumnTitle">Обои</div>
          <div class="footer__firstBlockColumnDescription">
            <div class="footer__firstBlockColumnDescriptionText">Цветы</div>
            <div class="footer__firstBlockColumnDescriptionText">Горы</div>
            <div class="footer__firstBlockColumnDescriptionText">Детские</div>
            <div class="footer__firstBlockColumnDescriptionText">Акварель</div>
            <div class="footer__firstBlockColumnDescriptionText">Геометрия</div>
            <div class="footer__firstBlockColumnDescriptionText">Градиенты</div>
            <div class="footer__firstBlockColumnDescriptionText">Модерн</div>
            <div class="footer__firstBlockColumnDescriptionText">Этника</div>
            <div class="footer__firstBlockColumnDescriptionText">Классика</div>
            <div class="footer__firstBlockColumnDescriptionText">Раскраски</div>
            <div class="footer__firstBlockColumnDescriptionText">Природа</div>
            <div class="footer__firstBlockColumnDescriptionText">
              Простые формы
            </div>
          </div>
        </div>
        <div class="footer__firstBlockColumn">
          <div class="footer__firstBlockColumnTitle">Плитка</div>
          <div class="footer__firstBlockColumnDescription">
            <div class="footer__firstBlockColumnDescriptionText">Тропики</div>
            <div class="footer__firstBlockColumnDescriptionText">
              Абстракция
            </div>
            <div class="footer__firstBlockColumnDescriptionText">Геометрия</div>
            <div class="footer__firstBlockColumnDescriptionText">Арт</div>
            <div class="footer__firstBlockColumnDescriptionText">Моноколор</div>
          </div>
        </div>
        <div class="footer__firstBlockColumn">
          <div class="footer__firstBlockColumnTitle">Краска</div>
          <div class="footer__firstBlockColumnDescription">
            <div class="footer__firstBlockColumnDescriptionText">
              Акцентные цвета
            </div>
            <div class="footer__firstBlockColumnDescriptionText">Тренды</div>
            <div class="footer__firstBlockColumnDescriptionText">
              Полная палитра
            </div>
            <div class="footer__firstBlockColumnDescriptionText">
              Готовые решения
            </div>
          </div>
        </div>
        <div class="footer__firstBlockColumn">
          <div class="footer__firstBlockColumnTitle">
            Стилистические подборки
          </div>
          <div class="footer__firstBlockColumnDescription">
            <div class="footer__firstBlockColumnDescriptionText">Природа</div>
            <div class="footer__firstBlockColumnDescriptionText">Цветы</div>
            <div class="footer__firstBlockColumnDescriptionText">Горы</div>
            <div class="footer__firstBlockColumnDescriptionText">Классика</div>
            <div class="footer__firstBlockColumnDescriptionText">Модерн</div>
            <div
              class="
                footer__firstBlockColumnDescriptionText
                footer__firstBlockColumnDescriptionText_beforeTitle
              "
            >
              Геометрия
            </div>
          </div>
          <div class="footer__firstBlockColumnTitle">
            Стилистические подборки
          </div>
          <div class="footer__firstBlockColumnDescription">
            <div class="footer__firstBlockColumnDescriptionText">Кисти</div>
            <div class="footer__firstBlockColumnDescriptionText">Клей</div>
            <div class="footer__firstBlockColumnDescriptionText">
              Системы укладки плитки
            </div>
          </div>
        </div>
        <div class="footer__firstBlockColumn">
          <div class="footer__firstBlockColumnTitle">Компания</div>
          <div class="footer__firstBlockColumnDescription">
            <div class="footer__firstBlockColumnDescriptionText">О нас</div>
            <div class="footer__firstBlockColumnDescriptionText">
              Дизайнерам
            </div>
            <div class="footer__firstBlockColumnDescriptionText">
              Оплата и доставка
            </div>
            <div class="footer__firstBlockColumnDescriptionText">
              Наш шоурум
            </div>
            <div class="footer__firstBlockColumnDescriptionText">
              Где купить
            </div>
            <div class="footer__firstBlockColumnDescriptionText">Контакты</div>
            <div class="footer__firstBlockColumnDescriptionText">Портфолио</div>
            <div class="footer__firstBlockColumnDescriptionText">
              <a
                class="
                  footer__firstBlockColumnDescriptionText
                  footer__firstBlockColumnDescriptionText_link
                "
                href="#"
                >Корпоративным клиентам</a
              >
            </div>
          </div>
        </div>
        <div class="footer__firstBlockColumn">
          <div class="footer__firstBlockColumnTitle">Контакты</div>
          <div class="footer__firstBlockColumnContacts">
            <div class="footer__firstBlockColumnContactItem">
              <img
                class="footer__firstBlockColumnContactItemSvg"
                fill="#CA3192"
                :src="require('@/assets/sprite/svg/phone.svg')"
              />
              <div class="footer__firstBlockColumnContactItemText">
                8 800 350 84 15
              </div>
            </div>
            <div class="footer__firstBlockColumnContactItem">
              <img
                class="footer__firstBlockColumnContactItemSvg"
                :src="require('@/assets/sprite/svg/mail.svg')"
              />
              <div class="footer__firstBlockColumnContactItemText">
                welcome@re-space.ru
              </div>
            </div>
          </div>
          <div class="footer__firstBlockColumnUnderline"></div>
          <div class="footer__firstBlockColumnSocial">
            <a href="#" class="footer__firstBlockColumnSocialLink">
              <img
                class="footer__firstBlockColumnSocialLinkSvg"
                :src="require('@/assets/sprite/svg/instagram_link.svg')"
              />
            </a>
            <a href="#" class="footer__firstBlockColumnSocialLink">
              <img
                class="footer__firstBlockColumnSocialLinkSvg"
                :src="require('@/assets/sprite/svg/facebook.svg')"
              />
            </a>
            <a href="#" class="footer__firstBlockColumnSocialLink">
              <img
                class="footer__firstBlockColumnSocialLinkSvg"
                :src="require('@/assets/sprite/svg/twitter.svg')"
              />
            </a>
            <a href="#" class="footer__firstBlockColumnSocialLink">
              <img
                class="footer__firstBlockColumnSocialLinkSvg"
                :src="require('@/assets/sprite/svg/pinterest.svg')"
              />
            </a>
            <a href="#" class="footer__firstBlockColumnSocialLink">
              <img
                class="footer__firstBlockColumnSocialLinkSvg"
                :src="require('@/assets/sprite/svg/youtube.svg')"
              />
            </a>
          </div>
          <div class="footer__firstBlockText">
            Соглашение об использовании сайта
          </div>
          <div class="footer__firstBlockText">© Respace 2012-2021</div>
        </div>
      </div>
      <div class="footer__secondBlock">
        <img
          class="footer__secondBlockSvg"
          @click="toTop"
          :src="require('@/assets/sprite/svg/arrow_up.svg')"
        />
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  methods: {
    toTop: function () {
      window.scrollTo({
        top: 0,
        left: 0,
        behavior: "smooth",
      });
    },
  },
};
</script>

<style lang="scss">
.footer__firstBlockColumnDescriptionText {
  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 34px;

  color: var(--colorBrown);

  &:last-child {
    margin: 0;
  }

  &_beforeTitle {
    margin: 0 0 26px 0;
  }

  &_link {
    color: var(--colorMoreContrastThanDullMagenta);
    text-decoration: none;
  }
}

.footer__firstBlock {
  display: flex;
  margin: 0 auto 81px auto;
  width: fit-content;
}

.footer__firstBlockColumn {
  width: 221px;
  margin: 0 15px 0 0;

  &:nth-child(4) {
    .footer__firstBlockColumnTitle {
      width: 180px;
      margin: 0 56px 16px 0;
    }

    .footer__firstBlockColumnDescription {
      margin: 0 0 26px 0;
    }
  }

  &:last-child {
    margin: 0;
  }
}

.footer__firstBlockColumnTitle {
  width: 221px;
  margin: 0 0 21px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;

  color: var(--colorPink);

  &:last-child {
    margin: 0 0 22px 0;
  }
}

.footer__firstBlockColumnContacts {
  display: grid;
}

.footer__firstBlockColumnContactItem {
  display: flex;
  align-items: center;
  margin: 0 0 8px 0;

  &:last-child {
    margin: 0 0 28px 0;
  }
}

.footer__firstBlockColumnContactItemSvg {
  display: flex;
  width: 15px;
  height: 15px;
  margin: 0 16px 0 0;

  filter: invert(28%) sepia(31%) saturate(3755%) hue-rotate(292deg)
    brightness(100%) contrast(96%);
}

.footer__firstBlockColumnContactItemText {
  display: flex;
  align-items: center;
  width: 190px;
  height: 24px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 60px;

  color: var(--colorPink);
}

.footer__firstBlockColumnUnderline {
  width: 221px;
  height: 0px;

  margin: 0 0 25px 0;

  border: 1px solid var(--colorPink);
}

.footer__firstBlockColumnSocial {
  display: flex;
  justify-content: space-between;
  width: 220px;
  margin: 0 0 31px 0;
}

.footer__firstBlockColumnSocialLink {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 35px;
  height: 35px;
  margin: 0 10px 0 0;

  border-radius: 100px;
  background: linear-gradient(90deg, #f880b9 0.29%, #ff98a6 100%);

  &:last-child {
    margin: 0;
  }
}

.footer__secondBlock {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto;
  width: 100%;

  background: linear-gradient(90deg, #9b4894 0%, #e94d94 51%, #f08b75 100%);
  transform: matrix(-1, 0, 0, 1, 0, 0);
}

.footer__secondBlockSvg {
  height: 30px;
  width: 16px;

  filter: invert(99%) sepia(1%) saturate(2624%) hue-rotate(177deg)
    brightness(123%) contrast(100%);
}

.footer__firstBlockText {
  margin: 0 0 13px 0;
  width: 205px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 24px;

  color: var(--colorBrown);
}

@media (max-width: 767px) {
  .footer__firstBlockColumn {
    display: none;
  }

  .footer__firstBlockColumn:nth-child(5) {
    display: block;
  }

  .footer__firstBlockColumn:nth-child(6) {
    display: block;
  }
}
</style>