<template>
  <div class="card__wrapper">
    <div class="card__imageWrapper">
      <img
        class="card__image"
        :src="require(`@/assets/images${image}`)"
        v-if="image"
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
    title: String,
    description: String,
  },
};
</script>

<style lang="scss">
.card {
  display: flex;
  align-items: center;
  height: 900px;

  background: var(--colorDarkerWhite);
}

.card__wrapper {
  display: flex;
  align-items: center;
  height: 900px;

  &:nth-child(even) {
    flex-direction: row-reverse;
  }
}

.card__imageWrapper {
  height: 900px;
}

.card__image {
  width: 960px;
  height: 900px;
}

.card__textWrapper {
  width: 899px;
  margin: 0 0 0 61px;
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

p {
  margin: 0 0 18px 0;
}
</style>