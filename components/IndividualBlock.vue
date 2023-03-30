<template>
  <div class="individualBlock__wrapper">
    <div class="individualBlock__text">
      <div class="individualBlock__image individualBlock__image_phone">
        <img
          :src="require('@/assets/images/individual-block-image-phone.png')"
          alt=""
        />
      </div>
      <div class="individualBlock__textTitle">
        Индивидуальный подход к каждому клиенту
      </div>
      <div
        class="individualBlock__textDescription individualBlock__textDescription_desktop"
      >
        <div class="individualBlock__textDescriptionText">
          Мы всегда готовы идти вам на встречу и обговаривать особые условия по
          производству, срокам и доставке. Дизайнерские обои Респейс — это не
          только качественный отделочный материал, это еще и сервис, который
          позволит вам быть уверенными в безупречном качестве и результате,
          который превзойдет ваши ожидания.
        </div>
        <div class="individualBlock__textDescriptionText">
          Наша главная задача в том, чтобы вы остались довольны и рекомендовали
          на своим друзьям и знакомым.
        </div>
      </div>
      <div
        class="individualBlock__textDescription individualBlock__textDescription_phone"
      >
        <div class="individualBlock__textDescriptionText">
          Мы всегда готовы идти вам на встречу и обговаривать особые условия по
          производству, срокам и доставке.
        </div>
        <div class="individualBlock__textDescriptionText" v-if="show">
          Дизайнерские обои Респейс — это не только качественный отделочный
          материал, это еще и сервис, который позволит вам быть уверенными в
          безупречном качестве и результате, который превзойдет ваши ожидания.
        </div>
        <div class="individualBlock__textDescriptionText" v-if="show">
          Наша главная задача в том, чтобы вы остались довольны и рекомендовали
          на своим друзьям и знакомым.
        </div>
      </div>
      <div
        class="individualBlock__textDescriptionButton"
        v-if="!show"
        @click="show = !show"
      >
        развернуть...
      </div>
      <div
        class="individualBlock__textDescriptionButton"
        v-if="show"
        @click="show = !show"
      >
        свернуть
      </div>
    </div>
    <div class="individualBlock__image individualBlock__image_desktop">
      <img class="individualBlock__imagePng"
        :src="require('@/assets/images/individual-block-image.png')"
        alt=""
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      show: false,
    };
  },
};
</script>

<style lang="scss">
.individualBlock__wrapper {
  display: flex;
  width: 1400px;
  margin: 0 260px 118px 260px;
}

.individualBlock__text {
  margin: 24px 61px 57px 0;
}

.individualBlock__image {
  width: 700px;
  height: 456px;

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

.individualBlock__textTitle {
  width: 583px;
  margin: 0 0 34px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: var(--colorDullMagenta);
}

.individualBlock__textDescription {
  width: 639px;

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

.individualBlock__textDescriptionText {
  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 27px;

  color: var(--colorBrown);
}

.individualBlock__textDescriptionButton {
  display: none;
}

@media (max-width: 1919px) {
  .individualBlock__wrapper {
    width: 1000px;
    margin: 0 auto 118px auto;
    align-items: center;
    padding: 0 12px 0 12px;
  }

  .individualBlock__image {
    width: auto;
    height: 358px;
  }

  .individualBlock__imagePng {
    width: 550px;
  }

  .individualBlock__text {
    margin: 24px auto 57px 0;
  }

  .individualBlock__textTitle {
    width: auto;
  }

  .individualBlock__textDescription {
    width: auto;
  }
}

@media (max-width: 1023px) {
  .individualBlock__wrapper {
    display: flex;
    width: 320px;
    margin: 0 auto 85px auto;
    justify-content: center;
  }

  .individualBlock__textTitle {
    width: 270px;
    margin: 0 auto 16px auto;

    font-weight: 500;
    font-size: 26px;
    line-height: 34px;
  }

  .individualBlock__textDescription {
    width: 270px;
    margin: 0 auto 16px auto;

    font-weight: 300;
    font-size: 16px;
    line-height: 27px;

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .individualBlock__textDescriptionButton {
    width: 270px;
    margin: 0 auto 46px auto;

    font-family: "Ubuntu";
    font-style: normal;
    font-weight: 300;
    font-size: 12px;
    line-height: 27px;

    color: var(--colorPink);
  }

  .individualBlock__image {
    width: 269px;
    height: 198px;
    margin: 45px auto 34px auto;

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .individualBlock__text {
    width: 320px;
    margin: 0 auto 46px auto;
  }
}
</style>