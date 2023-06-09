<template>
  <div id="app">
    <div class="dot-grid"></div>
      <div class="main">
        <div id="spectrum">
        <video autoplay muted loop>
          <source src="./assets/Orb.mp4" type="video/mp4">
          Your browser does not support the video tag.
        </video>
        <div class="glow-spehere"></div>
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
  background: rgb(1, 0, 27);
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

video {
  border-radius: 360px;
  height: 20rem;
  border: 1px solid rgba(128, 128, 128, 0.1);
}

.glow-spehere {
  height: 20rem;
  width: 20rem;
  background: rgb(120,173,255);
  background: radial-gradient(circle, rgba(120,173,255,1) 0%, rgb(103, 100, 255) 50%, rrgb(43, 0, 255)100%);
  position: absolute;
  top: calc(50% - 10rem - 0.5px);
  left: calc(50% - 10rem - 0.5px);
  border-radius: 50%;
  opacity: 0.1;
  box-shadow: 0px 0px 80px 30px rgb(94, 163, 236);
}
</style>