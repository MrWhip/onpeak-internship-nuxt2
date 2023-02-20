<template>
  <div class="social__wrapper">
    <div class="social__image">
      <img
        class="social__imageSvg"
        :src="require('@/assets/sprite/svg/instagram.svg')"
      />
    </div>
    <div class="social__text">
      <div class="social__textTitle">Респейс в Instagram</div>
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
  margin: 0 260px 144px 260px;
}

.social__text {
  width: 692px;
}

.social__image {
  margin: 0 47px 0 0;
}

.social__textTitle {
  margin: 0 0 36px 0;
  width: 692px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: var(--colorDullMagenta);
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
  backdrop-filter: blur(7.5px);

  border-radius: 10px;
}
</style>