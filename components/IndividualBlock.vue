<template>
  <div class="individualBlock__wrapper">
    <div class="individualBlock__text">
        <div class="individualBlock__textTitle">Индивидуальный подход к каждому клиенту</div>
        <div class="individualBlock__textDescription"><p>Мы всегда готовы идти вам на встречу и обговаривать особые условия по производству, срокам и доставке. Дизайнерские обои Респейс — это не только качественный отделочный материал, это еще и сервис, который позволит вам быть уверенными в безупречном качестве и результате, который превзойдет ваши ожидания.</p><p>Наша главная задача в том, чтобы вы остались довольны и рекомендовали на своим друзьям и знакомым.</p></div>
    </div>
    <div class="individualBlock__image">
        <img :src="require('@/assets/images/individual-block-image.png')" alt="" />
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.individualBlock__wrapper {
    display: flex;
    width: 1400px;
    margin: 0 260px 118px 260px;
}

.individualBlock__text {
    width: 639px;
    margin: 24px 61px 57px 0;
}

.individualBlock__image {
    width: 700px;
    height: 456px;
}

.individualBlock__textTitle {
    width: 583px;
    margin: 0 0 34px 0;

    font-family: 'Ubuntu';
    font-style: normal;
    font-weight: 500;
    font-size: 46px;
    line-height: 60px;

    color: var(--colorDullMagenta);
}

.individualBlock__textDescription {
    width: 639px;

    font-family: 'Ubuntu';
    font-style: normal;
    font-weight: 300;
    font-size: 18px;
    line-height: 27px;

    color: var(--colorBrown);
}
</style>