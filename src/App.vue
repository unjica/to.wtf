<template>
  <div class="background">
    <router-view />
  </div>
</template>

<style lang="scss">
@media only screen and (max-width: 760px) {
  .desktop {
    display: none !important;
  }
  .margin {
    margin: 0 20px;
  }
}
@media only screen and (min-width: 761px) {
  .mobile {
    display: none !important;
  }
  .margin {
    margin: 0 auto;
  }
}
@font-face {
  font-family: Alpina;
  src: url(./fonts/GT-Alpina-Standard-Thin.ttf);
}
@font-face {
  font-family: Cinetype;
  src: url(./fonts/GT-Cinetype-Mono.ttf);
}
.alpina {
  font-family: Alpina;
}
#app {
  font-family: Cinetype, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #0f2a63;
  background-color: #B3E6BE;
}
.container {
  max-width: 800px;
  margin: auto;
}
.hr {
  width: 100%;
  background-color: #0f2a63;
  height: 1px;
}
* {
  color: #0f2a63;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.background {
  background-image: url(./assets/background.svg);
  background-size: cover;
  background-repeat: no-repeat;
}
li {
  list-style: none;
  margin-left: 1.5em;
}
li::before {
  content: '';
  position: absolute;
  display: inline-block;
  height: 1em;
  width: 1em;
  transform: translate(-1.5em, 0.1em);
  background-image: url(./assets/arrow.png);
  background-size: contain;
  background-repeat: no-repeat;
}
</style>
