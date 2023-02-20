<template>
  <div class="wallpaper__wrapper">
    <div class="wallpaper__text">
      <div class="wallpaper__textTitle">Обои</div>
      <div class="wallpaper__textLink">
        <div class="wallpaper__textLinkTitle">Смотреть все обои</div>
        <div class="wallpaper__textImage">
          <img
            class="wallpaper__textImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
      </div>
    </div>
    <div class="wallpaper__columnsWrapper">
      <div class="wallpaper__column">
        <div class="wallpaper__card wallpaper__card_odd">
          <img
            class="wallpaper__cardImage"
            :src="require('@/assets/images/columns_images/1.png')"
          />
          <div class="wallpaper__cardText"></div>
        </div>
        <div class="wallpaper__columnDescription">Природа</div>
        <div class="wallpaper__columnDescriptionImage">
          <img
            class="wallpaper__columnDescriptionImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
        <div class="wallpaper__card_odd">
          <img
            class="wallpaper__cardImage"
            :src="require('@/assets/images/columns_images/2.png')"
          />
        </div>
        <div class="wallpaper__columnDescription">Геометрия</div>
        <div class="wallpaper__columnDescriptionImage">
          <img
            class="wallpaper__columnDescriptionImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
        <div class="wallpaper__card_odd wallpaper__card_last">
          <img
            class="wallpaper__cardImage wallpaper__cardImage_last"
            :src="require('@/assets/images/columns_images/3.png')"
          />
        </div>
        <div class="wallpaper__columnDescription">Цветы</div>
        <div class="wallpaper__columnDescriptionImage">
          <img
            class="wallpaper__columnDescriptionImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
      </div>
      <div class="wallpaper__column"></div>
      <div class="wallpaper__column">
        <div class="wallpaper__card_odd">
          <img
            class="wallpaper__cardImage"
            :src="require('@/assets/images/columns_images/6.png')"
          />
        </div>
        <div class="wallpaper__columnDescription">Градиенты</div>
        <div class="wallpaper__columnDescriptionImage">
          <img
            class="wallpaper__columnDescriptionImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
        <div class="wallpaper__card_odd">
          <img
            class="wallpaper__cardImage"
            :src="require('@/assets/images/columns_images/7.png')"
          />
        </div>
        <div class="wallpaper__columnDescription">Акварель</div>
        <div class="wallpaper__columnDescriptionImage">
          <img
            class="wallpaper__columnDescriptionImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
        <div class="wallpaper__card_odd wallpaper__card_last">
          <img
            class="wallpaper__cardImage wallpaper__cardImage_last"
            :src="require('@/assets/images/columns_images/8.png')"
          />
        </div>
        <div class="wallpaper__columnDescription">Обои для спальни</div>
        <div class="wallpaper__columnDescriptionImage">
          <img
            class="wallpaper__columnDescriptionImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
      </div>
      <div class="wallpaper__column">
        <div class="wallpaper__card_odd">
          <img
            class="wallpaper__cardImage"
            :src="require('@/assets/images/columns_images/9.png')"
          />
        </div>
        <div class="wallpaper__columnDescription">Детские</div>
        <div class="wallpaper__columnDescriptionImage">
          <img
            class="wallpaper__columnDescriptionImageSvg"
            :src="require('@/assets/sprite/svg/arrow_right.svg')"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.wallpaper__card {
  &:hover {
    .wallpaper__cardText {
      opacity: 1;
    }

    .wallpaper__cardImage {
      backdrop-filter: blur(4px);
      background: rgba(0, 0, 0, 0.3);
    }
  }
}

.wallpaper__cardText {
  opacity: 0;
  transition: all 500ms ease; 
}

.wallpaper__cardImage {
  opacity: 0;
  transition: all 500ms ease; 
}
</style>