<template>
  <router-view />
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Sawarabi+Gothic&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Arimo:wght@400;700&display=swap');
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  cursor: none;
  font-family: $font-family-standard;
  background-color: #000;  /* 背景の基本カラーは黒 */
  @include respond(tablet) {
    font-size: 87.5%; // 1rem == 14px
    cursor: default;
  }
  @include respond(phone) {
    font-size: 75%; // 1rem == 12px
  }
}
</style>
