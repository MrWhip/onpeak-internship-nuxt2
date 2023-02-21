<template>
  <div class="ceramicTiles__wrapper">
    <div class="ceramicTiles__textWrapper">
      <div class="ceramicTiles__Title">Керамическая плитка</div>
      <div class="ceramicTiles__Description">
        <div class="ceramicTiles__DescriptionText">
          Дизайнерская керамическая плитка – нестандартное, яркое решение,
          которое часто можно применить только в уникальных, идеальных по
          соблюдению стилистики помещениях. Такие коллекции часто выпускаются
          ограниченной серией или становятся единственными в своем роде.
        </div>
        <div class="ceramicTiles__DescriptionText">
          Керамическая плитка в интерьере выглядит достаточно стильно,
          оригинально, так как имеет матовую или глянцевую поверхность, а также
          разнообразную текстуру, орнамент и рисунок. Этот материал используется
          для отделки стен, потолков, кухонных фартуков и широко применяется в
          дизайне гостиной и ванной комнаты.
        </div>
      </div>
      <a href="#" class="ceramicTiles__Link">
        <div class="ceramicTiles__LinkDescription">Смотреть всю плитку</div>
        <div class="ceramicTiles__LinkImage">
          <img
            class="ceramicTiles__LinkSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
      </a>
    </div>
    <div class="ceramicTiles__image">
      <img
        class="ceramicTiles__imageSvg"
        :src="require('@/assets/images/ceramic.png')"
      />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.ceramicTiles__wrapper {
  display: flex;
  margin: 0 260px 73px 260px;
  width: 1400px;
}

.ceramicTiles__textWrapper {
  margin: 0 70px 0 0;
}

.ceramicTiles__Title {
  width: 600px;
  margin: 0 0 32px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: var(--colorDullMagenta);
}

.ceramicTiles__Description:last-of-type {
  margin: 0 0 55px 0;
}

.ceramicTiles__DescriptionText {
  width: 649px;
  margin: 0 0 27px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 27px;

  color: var(--colorBrown);
}

.ceramicTiles__Link {
  display: flex;
  width: 200px;
  align-content: center;
  text-decoration: none;
}

.ceramicTiles__LinkSvg {
  filter: invert(33%) sepia(51%) saturate(3113%) hue-rotate(300deg) brightness(82%) contrast(92%);
}

.ceramicTiles__LinkDescription {
  width: 190px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 16px;

  color: var(--colorPink);
}
</style>