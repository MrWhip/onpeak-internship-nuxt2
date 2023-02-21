<template>
  <div class="designerWallpaper">
    <div class="designerWallpaper__wrapper">
      <div class="designerWallpaper__text">
        <div class="designerWallpaper__title">
          Дизайнерские обои вашей мечты
        </div>
        <div class="designerWallpaper__description">
          Обои Респейс будут полностью соответствовать вашим пожеланиям или
          требованиям дизайн проекта. Привычный интерьер заиграет новыми
          красками, а если вы решили полностью обновить свою квартиру и делаете
          ремонт — дизайнерские обои Респейс на ваших стенах очаруют вас с
          первой же минуты.
        </div>
      </div>
      <video class="designerWallpaper__video">
        <source
          :src="require('@/assets/videos/arte.mp4')"
          type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'
        />
      </video>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style>
.designerWallpaper {
  display: flex;
  align-items: center;
  width: 100%;
  height: 658px;
  background: var(--colorDarkerWhite);
}

.designerWallpaper__wrapper {
  display: flex;
  margin: 0 auto;
  width: fit-content;
}

.designerWallpaper__text {
  margin: 0 133px auto auto;
}

.designerWallpaper__description {
  width: 457px;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 300;
  font-size: 18px;
  line-height: 27px;

  color: var(--colorBrown);
}

.designerWallpaper__title {
  width: 457px;
  margin: 0 0 34px 0;

  font-family: "Ubuntu";
  font-style: normal;
  font-weight: 500;
  font-size: 46px;
  line-height: 60px;

  color: var(--colorDullMagenta);
}

.designerWallpaper__video {
  width: 810px;
  height: 456px;

  border-radius: 0px 40px;
}
</style>