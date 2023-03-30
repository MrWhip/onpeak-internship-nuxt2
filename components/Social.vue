<template>
  <div class="social__wrapper">
    <div class="social__background"></div>
    <div class="social__image social__image_desktop">
      <img
        class="social__imageSvg social__imageSvg_desktop"
        :src="require('@/assets/sprite/svg/instagram.svg')"
      />
    </div>
    <div class="social__text">
      <div class="social__header">
        <div class="social__image social__image_phone">
          <img
            class="social__imageSvg social__imageSvg_phone"
            :src="require('@/assets/sprite/svg/instagram.svg')"
          />
        </div>
        <div class="social__textTitle social__textTitle_phone">
          Респейс в Instagram
        </div>
      </div>
      <div class="social__textTitle social__textTitle_desktop">
        Респейс в Instagram
      </div>
      <div class="social__textDescription">
        Подписывайтесь на наш Instagram, следите за новостями, мы публикуем
        много всего интересного! Все подписчики получают промо-код на скидку 5%!
      </div>
    </div>
    <a href="#" class="social__button">Подписаться</a>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.social__wrapper {
  display: flex;
  width: 1400px;
  margin: 0 auto 144px auto;
}

.social__header {
  display: none;
}

.social__text {
  width: 692px;
}

.social__image {
  margin: 0 47px 0 0;
}

.social__textTitle {
  margin: 0 0 36px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: var(--colorDullMagenta);
}

.social__background {
  display: none;
}

.social__textDescription {
  width: 574px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 28px;

  color: var(--colorBrown);
}

.social__button {
  width: 457px;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 22px;
  line-height: 25px;
  text-align: center;
  text-decoration: none;

  color: var(--colorWhite);
  margin: 105px 0 0 0;

  background: linear-gradient(90deg, #9b4894 0%, #e94d94 51%, #f08b75 100%);

  border-radius: 10px;
}

@media (max-width: 1919px) {
  .social__wrapper {
    width: 1024px;
    align-items: center;
  }
  .social__text {
    width: auto;
  }

  .social__imageSvg {
    width: 83px;
    height: 83px;
  }

  .social__button {
    margin: 0;
  }
}

@media (max-width: 1023px) {
  .social__wrapper {
    position: relative;
    width: 320px;
    display: grid;
    justify-content: space-around;
    justify-items: center;
    margin: 0 auto 79px auto;
  }

  .social__header {
    display: flex;

    margin-top: 57px;
  }

  .social__background {
    display: block;

    background: var(--colorDarkerWhite);
    backdrop-filter: blur(4px);

    position: absolute;
    z-index: -1;

    width: 320px;
    height: 100%;

    border-radius: 0px;
  }

  .social__text {
    width: 270px;
  }

  .social__textDescription {
    width: 271px;

    font-weight: 300;
    font-size: 16px;
    line-height: 26px;

    margin: 0 auto 31px auto;
  }

  .social__textTitle {
    font-weight: 500;
    font-size: 29px;
    line-height: 33px;

    &_desktop {
      display: none;
    }
  }

  .social__button {
    width: 97px;
    height: 18px;

    font-family: "Ubuntu";
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 18px;
    display: flex;
    align-items: center;
    text-align: center;
  }

  .social__imageSvg {
    width: 64px;
    height: 64px;
  }

  .social__image {
    &_desktop {
      display: none;
    }
  }

  .social__button {
    width: 270px;
    height: 56px;

    margin: 0 auto 54px auto;
  }
}
</style>