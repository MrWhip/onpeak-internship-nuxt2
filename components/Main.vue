<template>
  <div id="app" class="main">
    <div class="main__buttons">
      <button @click="removeSlide" v-if="index != 1" :disabled="(index = 1)">
        <img
          class="main__buttonSvg"
          :src="require('@/assets/sprite/svg/arrow_left.svg')"
        />
      </button>
      <button @click="addSlide" v-if="index != 4" :disabled="(index = 4)">
        <img
          class="main__buttonSvg"
          :src="require('@/assets/sprite/svg/arrow_left.svg')"
        />
      </button>
    </div>
    <div class="slides">
      <transition-group
        name="slide"
        mode="out-in"
        enter-class="slide-in"
        leave-class="slide-out"
        enter-active-class="animated slide-in-active"
        leave-active-class="animated slide-out-active"
      >
        <!-- <div v-for="index in slides" v-if="index == active" :key="index"> 
          Slide {{ index }}
        </div>-->
      </transition-group>
    </div>
    <span class="prev" @click="move(-1)">
      <i class="fa fa-chevron-left" aria-hidden="true"></i>
    </span>
    <span class="next" @click="move(1)">
      <i class="fa fa-chevron-right" aria-hidden="true"></i>
    </span>
    <ul class="dots">
      <!-- <li
        v-for="(dot, index) in slides"
        :class="{ active: ++index === active }"
        @click="jump(index)"
      ></li> -->
    </ul>
  </div>
</template>

<script>
export default {
  el: '#app',
  data: {
    slides: 4,
    active: 1,
  },
  methods: {
    move(amount) {
      let newActive
      const newIndex = this.active + amount
      if (newIndex > this.slides) newActive = 1
      if (newIndex === 0) newActive = this.slides
      this.active = newActive || newIndex
    },
    jump(index) {
      this.active = index
    },
    addSlide() {
      this.slides = this.slides + 1
    },
    removeSlide() {
      this.slides = this.slides - 1 
    }
  }
};
</script>

<style>
</style>