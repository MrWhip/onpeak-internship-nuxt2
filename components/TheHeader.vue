<template>
  <header>
    <div class="header">
      <div class="header__firstLine">
        <div class="header__firstLineWrapper">
          <div class="header__firstLineText">
            Доставка в любой город России всего 700 рублей. По Москве — 500
            рублей.
          </div>
          <div class="header__firstLineMailWrapper">
            <div class="header__firstLineMail">
              <img
                class="header__firstLineMailSvg"
                :src="require('@/assets/sprite/svg/mail.svg')"
              />
            </div>
            <div class="header__firstLineMailText">welcome@re-space.ru</div>
          </div>
          <div class="header__firstLinePhoneWrapper">
            <div class="header__firstLinePhone">
              <img
                class="header__firstLineMailSvg"
                :src="require('@/assets/sprite/svg/phone.svg')"
              />
            </div>
            <div class="header__firstLinePhoneNumber">8 800 350 84 15</div>
          </div>
        </div>
      </div>
      <div class="header__secondLine">
        <div class="header__secondLineWrapper">
          <div class="header__secondLineLogo">
            <img :src="require('@/assets/images/respace-logo.png')" alt="" />
          </div>
          <div class="header__secondLineLinksWrapper">
            <div class="header__secondLineLink">Обои</div>
            <div class="header__secondLineLink">Плитка</div>
            <div class="header__secondLineLink">Краски</div>
            <div class="header__secondLineLink">О компании</div>
            <div class="header__secondLineLink">Контакты</div>
          </div>
          <div class="header__secondLineDividingLine"></div>
          <div class="header__secondLineSearch">
            <img
              class="header__secondLineSearchSvg"
              :src="require('@/assets/sprite/svg/search.svg')"
            />
          </div>
          <a href="#" class="header__secondLineLike">
            <img
              class="header__secondLineLikeSvg"
              :src="require('@/assets/sprite/svg/Like.svg')"
            />
          </a>
          <a href="#" class="header__secondLineShoppingCart">
            <img
              class="header__secondLineShoppingCartSvg"
              :src="require('@/assets/sprite/svg/shopping-cart.svg')"
            />
            <div
              class="header__secondLineShoppingCartQuantity"
              v-if="!isCartEmpty"
            >
              {{ itemsInCart }}
            </div>
          </a>
          <a href="#" class="header__secondLineMenuText">Меню</a>
          <div class="header__secondLineMenuImage">
            <img
              class="header__secondLineMenuImageSvg"
              :src="require('@/assets/sprite/svg/menu.svg')"
            />
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      itemsInCart: 0,
    };
  },

  computed: {
    isCartEmpty() {
      return this.itemsInCart == 0;
    },
  },
};
</script>

<style lang="scss">
.header__firstLine {
  height: 40px;
  margin: 0 auto;
  width: 100%;

  background: linear-gradient(90deg, #9b4894 0%, #e94d94 51%, #f08b75 100%);
  transform: matrix(-1, 0, 0, 1, 0, 0);
}

.header__firstLineWrapper {
  display: flex;
  flex-direction: row;
  width: fit-content;
  margin: 0 auto;
  transform: matrix(-1, 0, 0, 1, 0, 0);
}

.header__firstLineText {
  height: 15px;
  margin: 13px 593px 12px 0;
  width: 468px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 13px;
  line-height: 15px;

  color: var(--colorWhite);
}

.header__firstLineMailWrapper {
  display: flex;
  align-items: center;
}

.header__firstLinePhoneWrapper {
  display: flex;
  align-items: center;
}

.header__firstLineMailSvg {
  display: flex;
  height: 15px;
  width: 15px;
  margin: 13px 6px 12px 0;
  border-radius: 0px;

  filter: invert(99%) sepia(1%) saturate(2624%) hue-rotate(177deg)
    brightness(123%) contrast(100%);
}

.header__firstLineMailText {
  margin: 8px 45px 8px 0;
  width: 144px;
  height: 24px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 60px;

  display: flex;
  align-items: center;

  color: var(--colorWhite);
}

.header__firstLinePhoneSvg {
  display: flex;
  width: 15px;
  height: 15px;

  margin: 12px 8px 13px 0;

  filter: invert(99%) sepia(1%) saturate(2624%) hue-rotate(177deg)
    brightness(123%) contrast(100%);
}

.header__secondLineDividingLine {
  margin: 22px 18px 22px 0;
  height: 36px;

  border: 1px solid var(--colorPink);
}

.header__firstLinePhoneNumber {
  margin: 8px 0 8px 0;
  height: 24px;
  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 60px;

  display: flex;
  align-items: center;

  color: var(--colorWhite);
}

.header__secondLineWrapper {
  display: flex;
  align-items: center;
  margin: 0 auto;
  width: fit-content;
}

.header__secondLineLogo {
  margin: 18px 148px 18px 0;
}

.header__secondLineLinksWrapper {
  width: 574px;
  margin: 0 133px 0 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.header__secondLineShoppingCart {
  display: flex;
  position: relative;
  height: 28px;
  width: 28px;
}

.header__secondLineShoppingCartQuantity {
  display: flex;
  border-radius: 100px;
  position: absolute;
  z-index: 1;
  width: 15px;
  height: 15px;
  top: -5px;
  right: -5px;
  align-items: center;
  justify-content: center;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 9px;

  color: var(--colorWhite);

  background-color: var(--colorPink);
}

.header__secondLineLink {
  display: flex;
  align-items: center;
  margin: 0 65px 0 0;
  height: 19px;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;

  color: var(--colorBrown);

  &:last-child {
    margin: 0;
  }
}

.header__secondLineSearch {
  margin: 30px 80px 30px 0;
}

.header__secondLineLike {
  text-decoration: none;
}

.header__secondLineLikeSvg {
  margin: 31px 29px 31px 0;
}

.header__secondLineShoppingCart {
  text-decoration: none;
  margin: 0 58px 0 0;
}

.header__secondLineShoppingCartSvg {
  display: flex;
  position: relative;
}

.header__secondLineMenuText {
  text-decoration: none;
  width: 45px;
  margin: 0 16px 0 0;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;

  color: var(--colorPink);
}
</style>