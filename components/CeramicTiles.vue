<template>
  <div class="ceramicTiles__wrapper">
    <div class="ceramicTiles__text">
      <div class="ceramicTiles__textTitle">Керамическая плитка</div>
      <div class="ceramicTiles__textDescription">
        Дизайнерская керамическая плитка – нестандартное, яркое решение, которое
        часто можно применить только в уникальных, идеальных по соблюдению
        стилистики помещениях. Такие коллекции часто выпускаются ограниченной
        серией или становятся единственными в своем роде.Керамическая
        плитка в интерьере выглядит достаточно стильно, оригинально, так как
        имеет матовую или глянцевую поверхность, а также разнообразную текстуру,
        орнамент и рисунок. Этот материал используется для отделки стен,
        потолков, кухонных фартуков и широко применяется в дизайне гостиной и
        ванной комнаты.
      </div>
      <a class="ceramicTiles__textLink">
        <div class="ceramicTiles__textLinkDescription">Смотреть всю плитку</div>
        <div class="ceramicTiles__textLinkImage">
          <img
            class="ceramicTiles__textLinkSvg"
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
export default {

}
</script>

<style>
.ceramicTiles__wrapper {
  margin: 0 260px 0 260px;
  width: 1400px;
}

.ceramicTiles__textTitle {
  width: 600px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: #843c6a;
}

.ceramicTiles__textDescription {
  width: 638px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 27px;

  color: var(--colorBrown);
}
</style>