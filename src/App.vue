<template>
  <div id="app">
    <div class="dot-grid"></div>
      <div class="main">
        <div id="spectrum">
        <video  autoplay muted loop>
          <source src="./assets/Orb.mp4" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
#app {

}
</style>

<style>
body {
  background: rgb(2,0,36);
  margin: 0;
}
.dot-grid {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: radial-gradient(#292d44 1px, transparent 1px);
  background-size: 40px 40px;
}

.main {
  position: absolute;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>