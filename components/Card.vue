<template>
  <div class="card__wrapper">
    <div class="card__imageWrapper card__imageWrapper_desktop">
      <img
        class="card__image"
        :src="require(`@/assets/images${image}`)"
        v-if="image"
      />
    </div>
    <div class="card__imageWrapper card__imageWrapper_phone">
      <img
        class="card__image"
        :src="require(`@/assets/images${imagePhone}`)"
        v-if="imagePhone"
      />
    </div>
    <div class="card__textWrapper">
      <div class="card__title">{{ title }}</div>
      <div class="card__description" v-html="description"></div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: String,
    imagePhone: String,
    title: String,
    description: String,
  },

  data() {
    return {
      show: false,
    };
  },
};
</script>

<style lang="scss">
.card {
  display: flex;
  align-items: center;
  height: auto;

  background: var(--colorDarkerWhite);
}

.card__wrapper {
  display: flex;
  align-items: center;
  height: auto;

  &:nth-child(even) {
    flex-direction: row-reverse;
  }
}

.card__imageWrapper {
  height: 900px;

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

.card__image {
  width: 960px;
  height: 900px;
}

.card__textWrapper {
  width: 899px;
  margin: 0 0 0 61px;
  height: auto;
}

.card__title {
  margin: 0 363px 32px 0;
  width: 536px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: var(--colorDullMagenta);
}

.card__description {
  width: 639px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 27px;

  color: var(--colorBrown);
}

.link {
  color: var(--colorPink);
  text-decoration: underline;
  text-decoration-color: var(--colorPink);
}

.card__textDescriptionButton {
  display: none;
}

p {
  margin: 0 0 18px 0;
}

@media (max-width: 767px) {
  .card__wrapper {
    display: block;
    width: 320px;
  }

  .card__imageWrapper {
    height: 300px;

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
      margin: 0 auto 29px auto;
    }
  }

  .card__textWrapper {
    width: 277px;
    height: auto;
    margin: 0 auto 61px auto;
  }

  .card__textDescriptionButton {
    display: block;
  }

  .card__image {
    width: 320px;
    height: 300px;
  }

  .card__title {
    width: 270px;
    margin: 0 auto 23px auto;

    font-weight: 500;
    font-size: 26px;
    line-height: 34px;
  }

  .card__description {
    width: 278px;

    font-weight: 300;
    font-size: 16px;
    line-height: 25px;
  }

  .card__textDescriptionButton {
    width: 73px;

    font-family: "Ubuntu";
    font-style: normal;
    font-weight: 300;
    font-size: 12px;
    line-height: 27px;

    color: var(--colorPink);
  }
}
</style>