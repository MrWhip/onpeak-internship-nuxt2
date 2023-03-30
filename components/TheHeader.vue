<template>
  <header>
    <div class="header">
      <div class="header__firstLine">
        <div class="header__firstLineWrapper">
          <div class="header__firstLineText header__firstLineText_desktop">
            Доставка в любой город России всего 700 рублей. По Москве — 500
            рублей.
          </div>
          <div class="header__firstLineText header__firstLineText_phone">
            Доставка по России - 700 ₽, по Москве - 500 ₽
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
          <div class="header__secondLineLogo header__secondLineLogo_desktop">
            <img
              class="header__secondLineLogoPng header__secondLineLogoPng_desktop"
              :src="require('@/assets/images/respace-logo.png')"
              alt=""
            />
          </div>
          <div class="header__secondLineLogo header__secondLineLogo_phone">
            <img
              class="header__secondLineLogoPng header__secondLineLogoPng_phone"
              :src="require('@/assets/images/respace-logo--mini.png')"
              alt=""
            />
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

  background: linear-gradient(90deg, #f08b75 0%, #e94d94 51%, #9b4894 100%);
}

.header__firstLineWrapper {
  display: flex;
  flex-direction: row;
  width: fit-content;
  margin: 0 auto;
}

.header__firstLineText {
  height: 15px;
  margin: 13px 593px 12px 0;

  font-family: "Roboto";
  font-style: normal;
  font-weight: 400;
  font-size: 13px;
  line-height: 15px;

  color: var(--colorWhite);

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
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
  margin: 8px 0;
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

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

.header__secondLineLinksWrapper {
  width: 574px;
  margin-right: 133px;
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
  margin-right: 65px;
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
  margin-right: 58px;
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

@media (max-width: 1919px) {
  .header__firstLineText {
    margin: 13px 100px 13px 0;
  }

  .header__secondLineLink {
    margin-right: 15px;
  }

  .header__secondLineLogo {
    margin: 18px 10px 18px 0;
  }

  .header__secondLineLinksWrapper {
    width: 400px;
    margin-right: 33px;
  }

  .header__secondLineSearch {
    margin: 30px 30px 30px 0;
  }

  .header__secondLineShoppingCart {
    margin-right: 30px;
  }
}

@media (max-width: 1023px) {
  .header {
    width: 100%; 
    margin: 0 auto;
  }

  .header__firstLineWrapper {
    width: 320px;
  }

  .header__firstLine {
    width: auto;
    height: 24px;
  }

  .header__firstLineText {
    display: grid;
    margin: 5px 34px 5px 25px;
    width: 261px;
    height: 14px;
    left: 25px;
    top: 5px;

    font-size: 12px;
    line-height: 14px;

    color: var(--colorWhite);

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .header__firstLineMailSvg {
    display: none;
  }

  .header__firstLineMailText {
    display: none;
  }

  .header__firstLinePhoneSvg {
    display: none;
  }

  .header__firstLinePhoneNumber {
    display: none;
  }

  .header__secondLineWrapper {
    width: 320px;
  }

  .header__secondLineLogo {
    margin: 19px 52px 19px 25px;

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .header__secondLineLogoPng {
    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .header__secondLineLinksWrapper {
    display: none;
  }

  .header__secondLineLink {
    display: none;
  }

  .header__secondLineSearch {
    display: none;
  }

  .header__secondLineDividingLine {
    display: none;
  }

  .header__secondLineMenuText {
    display: none;
  }

  .header__secondLineLike {
    margin: 23px 24px 22px 0;
  }

  .header__secondLineLikeSvg {
    margin: 0;
  }

  .header__secondLineShoppingCart {
    margin: 22px 26px 21px 0;
  }

  .header__secondLineShoppingCartSvg {
    width: 21px;
    height: 21px;
  }

  .header__secondLineShoppingCartQuantity {
    width: 15px;
    height: 15px;
  }
}
</style>