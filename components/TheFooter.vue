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
            <div class="footer__firstBlockColumnDescriptionText footer__firstBlockColumnDescriptionText_last">
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
            <div class="footer__firstBlockColumnDescriptionText footer__firstBlockColumnDescriptionText_beforeTitle">
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
              <a class="footer__firstBlockColumnDescriptionText footer__firstBlockColumnDescriptionText_link" href="#"
                >Корпоративным клиентам</a
              >
            </div>
          </div>
        </div>
        <div class="footer__firstBlockColumn_last">
          <div class="footer__firstBlockColumnTitle">Контакты</div>
          <div class="footer__firstBlockColumnContacts">
            <div class="footer__firstBlockColumnPhone">
              <svg-icon class="footer__firstBlockColumnPhoneSvg" name="phone" />
              <div class="footer__firstBlockColumnPhoneNumber">
                8 800 350 84 15
              </div>
            </div>
            <div class="footer__firstBlockColumnMail">
              <svg-icon class="footer__firstBlockColumnMailSvg" name="mail" />
              <div class="footer__firstBlockColumnMailText">
                welcome@re-space.ru
              </div>
            </div>
          </div>
          <div class="footer__firstBlockColumnUnderline"></div>
          <div class="footer__firstBlockColumnSocial">
            <div class="footer__firstBlockColumnSocialLink"></div>
            <div class="footer__firstBlockColumnSocialLink"></div>
            <div class="footer__firstBlockColumnSocialLink"></div>
            <div class="footer__firstBlockColumnSocialLink"></div>
            <div class="footer__firstBlockColumnSocialLink footer__firstBlockColumnSocialLink_last"></div>
          </div>
        </div>
      </div>
      <div class="footer__secondBlock">
        <svg-icon class="footer__secondBlockSvg" name="arrow_up" />
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
.footer__firstBlockColumnDescriptionText {
  margin: 0 0 17px 0;
}

.footer__firstBlockColumnDescriptionText_last {
  margin: 0;
}

.footer__firstBlockColumnDescriptionText_beforeTitle {
  margin: 0 0 26px 0;
}

.footer__firstBlockColumnDescriptionText_link {
  color: #c64b95;
  text-decoration: none;
}

.footer__firstBlock {
  display: flex;
  margin: 0 260px 81px 260px;
}

.footer__firstBlockColumn {
  width: 221px;
  margin: 0 15px 0 0;
}

.footer__firstBlockColumnTitle {
  width: 221px;
  margin: 0 0 16px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;

  color: #ca3192;
}

.footer__firstBlockColumnContacts {
  display: grid;
}

.footer__firstBlockColumnPhone {
  display: flex;

  width: 190px;
  margin: 0 0 8px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;

  color: #ca3192;
}

.footer__firstBlockColumnPhoneSvg {
  display: flex;
  width: 15px;
  height: 15px;
  margin: 0 16px 0 0;
}

.footer__firstBlockColumnMail {
  display: flex;

  width: 190px;
  margin: 0 0 28px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;

  color: #ca3192;
}

.footer__firstBlockColumnMailSvg {
  display: flex;
  width: 15px;
  height: 15px;
  margin: 0 16px 0 0;
}

.footer__firstBlockColumnUnderline {
  width: 221px;
  height: 0px;

  margin: 0 0 25px 0;

  border: 1px solid #ca3192;
}

.footer__firstBlockColumnSocial {
  display: flex;
  justify-content: space-between;
  width: 220px;
  margin: 0 0 31px 0;
}

.footer__firstBlockColumnSocialLink {
  width: 35px;
  height: 35px;
  margin: 0 10px 0 0;

  border-radius: 100px;
  background: linear-gradient(90deg, #f880b9 0.29%, #ff98a6 100%);
}

.footer__firstBlockColumnSocialLink_last {
  margin: 0;
}

.footer__secondBlock {
  display: flex;
  align-items: center;
  height: 60px;

  background: linear-gradient(90deg, #9b4894 0%, #e94d94 51%, #f08b75 100%);
  transform: matrix(-1, 0, 0, 1, 0, 0);
}

.footer__secondBlockSvg {
  height: 30px;
  width: 16px;
}
</style>