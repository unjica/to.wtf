<template>
  <div style="background-color: #B3E6BE;">
    <div style="padding: 0 10px; display: flex; justify-content: space-between; align-content: center;" class="container">
      <div>
        <img width="100" src="../assets/logo.png" alt="logo" class="image">
      </div>
      <div>
        <div class="menu">
          <span class="line"></span>
          <span class="line2"></span>
          <span class="line3"></span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<style scoped>
.image {
  top: -15px;
  position: absolute;
}
.menu {
  margin: 10px 0;
  width: 30px;
  height: 30px;
  border-radius: 20px;
  border: 1px solid #0f2a63;
  padding: 5px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
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
