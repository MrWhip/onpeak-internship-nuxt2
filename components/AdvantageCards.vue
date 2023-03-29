<template>
  <div class="advantageCard__wrapper">
    <div class="advantageCard__background"></div>
    <div class="advantageCard__secodlineDivindingLine"></div>
    <div class="advantageCard__titleWrapper">
      <img class="advantageCard__image" :src="require(`@/assets/images${image}`)" v-if="image" />
      <div class="advantageCard__title">{{ title }}</div>
      <div class="advantageCard__more" v-if="!show" @click="show = !show">
        <img class="advantageCard__moreSvg" :src="require(`@/assets/sprite/svg/arrow_down_mini.svg`)" />
      </div>
      <div class="advantageCard__more" v-if="show" @click="show = !show">
        <img class="advantageCard__moreSvg" :src="require(`@/assets/sprite/svg/arrow_up_mini.svg`)" />
      </div>
    </div>
    <div class="advantageCard__textWrapper">
      <div class="advantageCard__description advantageCard__description_phone" v-if="show" v-html="description"></div>
      <div class="advantageCard__description advantageCard__description_desktop" v-html="description"></div>
    </div>
    <div class="advantageCards__titleDividingLine"></div>
  </div>
</template>

<script>
export default {
  props: {
    image: String,
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
.advantageCard__titleWrapper {
  display: flex;
  align-items: flex-end;
  margin: 0 0 16px 0;
}

.advantageCard__image {
  margin: 0 26px 0 0;
}

.advantageCard__more {
  display: none;
}

.advantageCard__secodlineDivindingLine {
  display: none;
}

.advantageCards__titleDividingLine {
  display: none;
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

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

.advantageCard__background {
  display: none;
}

@media (max-width: 767px) {
  .advantageCard {
    width: 320px;
    margin: 0 auto 0 auto;
  }

  .advantageCard__background {
    display: block;

    background: var(--colorDarkerWhite);
    backdrop-filter: blur(4px);
  }

  .advantageCard__titleWrapper {
    display: flex;
    align-items: center;
    margin: 0 auto 0 auto;
  }

  .advantageCards__titleDividingLine {
    display: block;
  }

  .advantageCard__textWrapper {
    width: 320px;
    margin: 0 auto 0 auto;

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .advantageCard__image {
    width: 30.66px;
    height: 30px;
    margin: 10px 11px 10px 26px;
  }

  .advantageCard__title {
    width: 202px;
    margin: 0 18px 0 0;

    font-weight: 500;
    font-size: 12px;
    line-height: 14px;
  }

  .advantageCard__description {
    width: 267px;
    margin: 10px auto 16px auto;

    font-weight: 300;
    font-size: 12px;
    line-height: 22px;

    &_phone {
      display: block;
    }

    &_desktop {
      display: none;
    }
  }

  .advantageCard__secodlineDivindingLine {
    display: block;
  }

  .advantageCard__more {
    display: block;
  }
}
</style>