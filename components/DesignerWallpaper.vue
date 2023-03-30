<template>
  <div class="designerWallpaper">
    <div
      class="designerWallpaper__background designerWallpaper__background_desktop"
    ></div>
    <div class="designerWallpaper__wrapper">
      <div
        class="designerWallpaper__background designerWallpaper__background_phone"
      ></div>
      <div class="designerWallpaper__text">
        <div class="designerWallpaper__videoWrapper">
          <video
            class="designerWallpaper__video designerWallpaper__video_phone"
            @click="togglePlay"
            ref="videoPlayer"
          >
            <source
              :src="require('@/assets/videos/arte.mp4')"
              type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'
            />
          </video>
          <div
            class="designerWallpaper__videoButton designerWallpaper__videoButton_phone"
            @click="togglePlay"
            v-show="videoPaused"
          >
            <img
              class="designerWallpaper__videoButtonSvg"
              :src="require('@/assets/sprite/svg/play-button.svg')"
            />
          </div>
        </div>
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
      <div class="designerWallpaper__videoWrapper">
        <video
          class="designerWallpaper__video designerWallpaper__video_desktop"
          @click="togglePlay"
          ref="videoPlayer"
        >
          <source
            :src="require('@/assets/videos/arte.mp4')"
            type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'
          />
        </video>
        <div
          class="designerWallpaper__videoButton designerWallpaper__videoButton_desktop"
          @click="togglePlay"
          v-show="videoPaused"
        >
          <img
            class="designerWallpaper__videoButtonSvg"
            :src="require('@/assets/sprite/svg/play-button.svg')"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      videoPaused: true,
    };
  },

  methods: {
    togglePlay() {
      const video = this.$refs.videoPlayer;

      if (video.paused) {
        video.play();
        this.videoPaused = false;
      } else {
        video.pause();
        this.videoPaused = true;
      }
    },
  },
};
</script>

<style lang="scss">
.designerWallpaper {
  position: relative;
  display: flex;
  align-items: center;
  margin: 0 auto 167px auto;
}

.designerWallpaper__wrapper {
  display: flex;
  margin: 0 auto;
  width: fit-content;
  padding: 117px 0 85px 0;
}

.designerWallpaper__videoWrapper {
  position: relative;
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

.designerWallpaper__videoButton {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.1);
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 0 40px;

  &_desktop {
    display: flex;
  }

  &_phone {
    display: none;
  }
}

.designerWallpaper__videoButtonSvg {
  width: 80px;

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

.designerWallpaper__background {
  position: absolute;
  z-index: -1;
  width: 100%;
  backdrop-filter: blur(4px);
  height: 100%;
  background: var(--colorDarkerWhite);

  &_desktop {
    display: block;
  }

  &_phone {
    display: none;
  }
}

@media (max-width: 1919px) {
  .designerWallpaper__wrapper {
    width: 1024px;
  }

  .designerWallpaper__text {
    padding: 0 16.75px;
    margin: 0;
  }

  .designerWallpaper__video {
    width: 500px;
    height: 282px;
    border-radius: 0px 30px;
  }

  .designerWallpaper__videoWrapper {
    padding: 0;
    margin: 0;
  }

  .designerWallpaper__videoButtonSvg {
    width: 60px;
  }

  .designerWallpaper__videoButton{
    border-radius: 0 30px;
  }
}

@media (max-width: 1023px) {
  .designerWallpaper {
    margin: 0 auto 80px auto;
  }

  .designerWallpaper__video {
    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
      width: 274px;
      height: 154px;
      margin: 35px auto 34px auto;
      border-radius: 0px 10px;
    }
  }

  .designerWallpaper__wrapper {
    position: relative;
    width: 320px;
    padding: 0;
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

  .designerWallpaper__background {
    width: 320px;

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .designerWallpaper__videoButtonSvg {
    width: 32px;
    height: 32px;

    &_desktop {
      display: none;
    }

    &_phone {
      display: block;
    }
  }

  .designerWallpaper__videoButton {
    border-radius: 0 10px;

    &_desktop {
      display: none;
    }

    &_phone {
      display: flex;
    }
  }
}
</style>