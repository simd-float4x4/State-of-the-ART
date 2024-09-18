<template>
  <div>
    <div class="gradation-main">
      <img class="container" alt="背景画像" src="../assets/mpa-bagkcround-cover-halfsize.png">
    </div>
    <br>
    <div class="user_area ml-16 mb-32">
      <img class="icon_image" alt="アイコン画像" src="../assets/icon.png">
      <div class="ml-8">
        <h2>65922(simd-float4x4)</h2>
        <p class="l-lg-gray">Software Enginieer</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
    .container {
        width: var(--full-width);
        margin-top: var(--header-height);
    }

    .gradation-main {
        position: relative;
    }

    .gradation-main::before {
        content: "";
        position: absolute;
        width: var(--full-width);
        height: 100%;
        top: var(--zero);
        left: var(--zero);
        background: linear-gradient(var(--rotate-top), var(--main-bg-color), transparent);
    }

    .icon_image {
      width: 48px;
      height: 48px;
      border-radius: var(--corner-radius-half);
      border: var(--border-double-thin) solid white;
    }

    .user_area {
      display: flex;
    }
</style>