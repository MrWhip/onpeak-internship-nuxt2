<template>
  <div class="advantageCard__wrapper">
    <div class="advantageCard__titleWrapper">
      <img
        class="advantageCard__image"
        :src="require(`@/assets/images${image}`)"
        v-if="image"
      />
      <div class="advantageCard__title">{{ title }}</div>
    </div>
    <div class="advantageCard__textWrapper">
      <div class="advantageCard__description" v-html="description"></div>
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
.advantageCard__titleWrapper {
  display: flex;
  align-items: flex-end;
  margin: 0 0 16px 0;
}

.advantageCard__image {
    margin: 0 26px 0 0;
}

.advantageCard__title {
  width: 298px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 24px;
  line-height: 28px;
  letter-spacing: 0.1em;
  text-transform: uppercase;

  color: var(--colorBrown);
}

.advantageCard__textWrapper {
  width: 416px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 27px;

  color: var(--colorBrown);
}
</style>