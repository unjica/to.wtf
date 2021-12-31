<template>
  <div class="background">
    <router-view />
  </div>
</template>

<style lang="scss">
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
  background-color: #d9dbda;
}
.container {
  max-width: 800px;
  margin: auto
}
.hr {
  width: 100%;
  background-color: #0f2a63;
  height: 1px;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.background {
  background-image: url(./assets/background.png);
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
