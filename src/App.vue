<template>
  <div>
    <HeaderView></HeaderView>
    <ProfileView></ProfileView>
    <StackView></StackView>
    <CareerView></CareerView>
    <PortfolioView></PortfolioView>
    <CopyRightsView></CopyRightsView>
  </div>

  <footer class="mt-32">©︎simd-float4x4, 2024</footer>
</template>

<script>
import HeaderView from "./components/HeaderView.vue";
import ProfileView from "./components/ProfileView.vue";
import StackView from "./components/Stack/StackView.vue";
import CareerView from "./components/Career/CareerView.vue";
import PortfolioView from "./components/Portfolio/PortfolioView.vue";
import CopyRightsView from "./components/CopyRightsView.vue";

export default {
  name: 'App',
  components: {
    HeaderView,
    ProfileView,
    StackView,
    CareerView,
    PortfolioView,
    CopyRightsView
  }
}
</script>

<style>
  :root {
    /* 色に関するプロパティ */
    --main-bg-color: #1E1E1E;
    --main-color: #F7F7F7;
    --accent-color: red;
    --black-color: #000000;
    --light-gray-color: #BBBBBB;

    /* 角度に関するプロパティ */
    --rotate-top: 0deg;
    --rotate-traiing: 90deg;
    --rotate-leading: 270deg;
    --rotate-bottom: 180deg;

    /* 幅と高さに関するプロパティ */
    --full-width: 100%;
    --three-quarters-width: 75%;
    --half-width: 50%;
    --one-quarters-width: 25%;

    --header-height: 74px;
    --zero: 0;

    /* marginに関するプロパティ */
    --margin-extreme: 64px;
    --margin-big: 32px;
    --margin-default: 16px;
    --margin-medium: 10px;
    --margin-small: 8px;
    --margin-extra-small: 4px;

    /* borderに関するプロパティ */
    --border-ultra-thin: 1px;
    --border-thin: 2px;
    --border-double-thin: 4px;
    --border-medium: 8px;
    --border-double-medium: 16px;

    /* corner-radiusに関するプロパティ */
    --corner-radius-one-quarter: 25%;
    --corner-radius-half: 50%;
    --corner-radius-three-quarter: 75%;
    --corner-radius-fixed: 16px;

  }

  * {
    margin: 0;
    padding: 0;
    background-color: var(--main-bg-color);
    color: var(--main-color);
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  .section-title {
    margin: var(--margin-medium);
  }

  .l-lg-gray {
    color: var(--light-gray-color);
  }

  .ml-8 {
    margin-left: var(--margin-small);
  }

  .ml-16 {
    margin-left: var(--margin-default);
  }

  .mt-32 {
    margin-top: var(--margin-big);
  }

  .mb-32 {
    margin-bottom: var(--margin-big);
  }

  footer {
    width: var(--full-width);
    display: flex;
    justify-content: center;
  }
</style>