<template>
  <div class="ceramicTiles__wrapper">
    <div class="ceramicTiles__textWrapper">
      <div class="ceramicTiles__image ceramicTiles__image_phone">
        <img class="ceramicTiles__imageSvg" :src="require('@/assets/images/ceramic-phone.png')" />
      </div>
      <div class="ceramicTiles__title">Керамическая плитка</div>
      <div class="ceramicTiles__description">
        <div class="ceramicTiles__descriptionText">
          Дизайнерская керамическая плитка – нестандартное, яркое решение,
          которое часто можно применить только в уникальных, идеальных по
          соблюдению стилистики помещениях. Такие коллекции часто выпускаются
          ограниченной серией или становятся единственными в своем роде.
        </div>
        <div class="ceramicTiles__descriptionText" v-if="show">
          Керамическая плитка в интерьере выглядит достаточно стильно,
          оригинально, так как имеет матовую или глянцевую поверхность, а также
          разнообразную текстуру, орнамент и рисунок. Этот материал используется
          для отделки стен, потолков, кухонных фартуков и широко применяется в
          дизайне гостиной и ванной комнаты.
        </div>
        <div class="ceramicTiles__descriptionTextButton" v-if="!show" @click="show = !show">
          развернуть...
        </div>
        <div class="ceramicTiles__descriptionTextButton" v-if="show" @click="show = !show">
          свернуть
        </div>
      </div>
      <a href="#" class="ceramicTiles__link">
        <div class="ceramicTiles__linkDescription">Смотреть всю плитку</div>
        <div class="ceramicTiles__linkImage">
          <img class="ceramicTiles__linkSvg" :src="require('@/assets/sprite/svg/arrow_right.svg')" />
        </div>
      </a>
    </div>
    <div class="ceramicTiles__image ceramicTiles__image_desktop">
      <img class="ceramicTiles__imageSvg" :src="require('@/assets/images/ceramic.png')" />
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
.ceramicTiles__wrapper {
  display: flex;
  margin: 0 auto 73px auto;
  width: 1400px;
}

.ceramicTiles__image {
  &_phone {
    display: none;
  }
}

.ceramicTiles__textWrapper {
  margin-right: 60px;
}

.ceramicTiles__descriptionTextButton {
  display: none;
}

.ceramicTiles__title {
  width: 600px;
  margin-bottom: 32px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: var(--colorDullMagenta);
}

.ceramicTiles__description:last-of-type {
  margin-bottom: 55px;
}

.ceramicTiles__descriptionText {
  width: 649px;
  margin-bottom: 27px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 27px;

  color: var(--colorBrown);
}

.ceramicTiles__link {
  display: flex;
  width: 200px;
  align-content: center;
  text-decoration: none;
}

.ceramicTiles__linkSvg {
  filter: invert(33%) sepia(51%) saturate(3113%) hue-rotate(300deg) brightness(82%) contrast(92%);
}

.ceramicTiles__linkDescription {
  width: 190px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 16px;

  color: var(--colorPink);
}

@media (max-width: 1919px) {
  .ceramicTiles__wrapper {
    width: 1024px;
  }

  .ceramicTiles__title {
    width: auto;
  }

  .ceramicTiles__descriptionText {
    width: auto;
  }

  .ceramicTiles__imageSvg {
    width: 550px;
  }

  .ceramicTiles__textWrapper {
    padding: 0 20px;
    margin-right: 0;
  }
}

@media (max-width: 1023px) {
  .ceramicTiles__wrapper {
    width: 320px;
    display: flex;
    margin: 0 auto 0 auto;
    justify-content: center;
  }

  .ceramicTiles__imageSvg {
    width: 320px;
  }

  .ceramicTiles__textWrapper {
    margin: 0 auto 0 auto;
  }

  .ceramicTiles__image {
    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
      margin: 0 auto 35px auto;
    }
  }

  .ceramicTiles__link {
    display: none;
  }

  .ceramicTiles__title {
    width: 267px;
    margin: 0 auto 28px auto;
    font-weight: 500;
    font-size: 26px;
    line-height: 30px;
  }

  .ceramicTiles__descriptionText {
    width: 267px;
    margin: 0 auto 16px auto;

    font-weight: 300;
    font-size: 16px;
    line-height: 27px;
  }

  .ceramicTiles__descriptionTextButton {
    display: block;
    width: 267px;
    margin: 0 auto 54px auto;

    font-family: "Ubuntu";
    font-style: normal;
    font-weight: 300;
    font-size: 12px;
    line-height: 27px;

    color: var(--colorPink);
  }
}
</style>