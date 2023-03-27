<template>
  <div class="designerWallpaper">
    <div class="designerWallpaper__wrapper">
      <div class="designerWallpaper__text">
        <video class="designerWallpaper__video designerWallpaper__video_phone">
          <source
            :src="require('@/assets/videos/arte.mp4')"
            type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'
          />
        </video>
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
      <video class="designerWallpaper__video designerWallpaper__video_desktop">
        <source
          :src="require('@/assets/videos/arte.mp4')"
          type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'
        />
      </video>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.designerWallpaper {
  display: flex;
  align-items: center;
  height: 658px;
  margin: 0 auto 304px auto;
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

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

@media (max-width: 767px) {
  .designerWallpaper {
    margin: 0 auto 80px auto;
  }

  .designerWallpaper__video {
    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
      width: 275px;
      height: 152px;
      margin: 35px auto 34px auto;
      border-radius: 0px 10px;
    }
  }

  .designerWallpaper__wrapper {
    width: 320px;
  }

  .designerWallpaper__title {
    width: 275px;
    margin: 0 auto 23px auto;

    font-weight: 500;
    font-size: 26px;
    line-height: 38px;
  }

  .designerWallpaper__description {
    width: 275px;
    margin: 0 auto 50px auto;

    font-weight: 300;
    font-size: 16px;
    line-height: 27px;
  }

  .designerWallpaper__text {
    margin: 0 auto 0 auto;
  }
}
</style>