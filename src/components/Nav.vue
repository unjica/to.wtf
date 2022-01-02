<template>
  <div style="background-color: #B3E6BE; z-index: 3; position: sticky; top: 0">
    <div style="padding: 0 10px; display: flex; justify-content: space-between; align-content: center;" class="container">
      <div>
        <img :class="(scrollY < 0.00000001) ? 'image' : 'image scale'" src="../assets/logo.svg" alt="logo">
      </div>
      <div style="display: flex; justify-content: center; align-items: center">
        <div v-if="!menu" @click="$emit('openMenu')" class="menu">
          <span class="line"></span>
          <span class="line2"></span>
          <span class="line3"></span>
        </div>
        <div v-else @click="$emit('closeMenu')" class="menu" style="padding: 5px">
          <h2>X</h2>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Nav',
  props: ['menu'],
  data () {
    return {
      scrollY: 0
    }
  },
  created () {
    window.addEventListener('scroll', this.handleScroll)
  },
  unmounted () {
    window.removeEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll () {
      this.scrollY = window.scrollY
    }
  }
}
</script>

<style scoped>
.image {
  width: 70px;
  margin: 10px 0;
  transition: 0.4s;
}
.scale {
  width: 40px;
  margin: 5px 0;
  transition: 0.4s;
}
.menu {
  width: 30px;
  height: 30px;
  border-radius: 20px;
  border: 1px solid #0f2a63;
  padding: 5px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  cursor: pointer;
  transition: 0.2s;
}
.menu:hover {
  background-color: rgba(15, 42, 99, .1);
  transition: 0.2s;
}
.line {
  width: 15px;
  height: 2px;
  background-color: #0f2a63;
}
.line2 {
  width: 15px;
  height: 2px;
  background-color: #0f2a63;
}
.line3 {
  width: 15px;
  height: 2px;
  background-color: #0f2a63;
}
</style>
