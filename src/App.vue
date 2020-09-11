<template>
  <div id="app">
    <div class="anim">
      <div id="cont" style="margin-top:0">
        <!-- <video id="vid" width="auto" height="1750px" style="padding-top: 173px; padding-left: 50px" autoplay muted>
          <source src="./assets/videos/Fabric_UI_Animation_State 4.mp4" type="video/mp4">
          Your browser does not support the video tag. -->
        <!-- </video> -->
      </div>
      <img id="a1" src="./assets/Images/dashboard@3x.png">
      <img id="a2" src="./assets/Images/Dashboard_yellow_1@3x.png">
      <img id="a3" src="./assets/Images/Dashboard_red_2@3x.png">
      <img id="a4" style="z-index: 1; padding-right:785px; padding-top: 315px" src="./assets/Images/prod 1@3x.png">
      <img id="a5" src="./assets/Images/Dashboard_green_3@3x.png">
      <img id="a6" style="z-index: 1; padding-left:985px; margin-top: 465px;" src="./assets/Images/prod 2@3x.png">
      <img id="a7" style="z-index: 1; padding-left:1530px; padding-top:650px;" src="./assets/Images/prod 3@3x.png">
      <img id="a8" style="z-index: 1; padding-left:465px; padding-top:265px;" src="./assets/Images/prod 4@3x.png">
      <img id="a9" style="z-index: 1; margin-left:-670px; margin-top:260px;" src="./assets/Images/prod 5@3x.png">
      <img id="a10" style="z-index: -1; margin-left:-1640px; padding-top:120px;" src="./assets/Images/prod 6@3x.png">
      <div id="t1a11-vl" class="vl green-ot" style="margin-top: 460px; margin-right: 40px"></div>
      <div id="t1a11" class="tx green" style="z-index: 1; margin-top:405px; padding-left: 110px; width: 150px">
        <div style="padding-left: 32px">
          <h1>UI Tool 1</h1>
          <h1>description</h1>
        </div>
      </div>
      <div id="t2a12-hl" class="hl yellow-ot" style="margin-top: 1180px; margin-left: 1200px"></div>
      <div id="t2a12" class="tx yellow" style="z-index: 1; padding-top:210px; padding-left: 1580px; width: 150px">
        <div style="padding-left: 32px">
          <h1>UI Tool 2</h1>
          <h1>description</h1>
        </div>
      </div>
       <div id="t3a13-vl" class="vl red-ot" style="margin-top: 485px; margin-right: 2050px; height: 208px"></div>
      <div id="t3a13" class="tx red" style="z-index: 1; margin-top:180px; padding-right: 1900px; width: 150px">
        <div style="padding-left: 32px">
          <h1>UI Tool 3</h1>
          <h1>description</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import gsap from 'gsap'

export default {
  name: 'App',
  mounted(){
    // document.getElementById('vid').play();

    gsap.from('.anim', {opacity: 0, duration: 9, scale: 0.8, ease: "power4.out"})
    gsap.from('#a2', {opacity: 0, duration: 0.8, delay: 1.4, ease: "power4.out"})
    gsap.from('#a3', {opacity: 0, duration: 0.5, delay: 1.9, ease: "power4.out"})
    gsap.from('#a4', {opacity: 0, duration: 1.2, y: 70, delay: 2.1, ease: "power4.out"})
    gsap.from('#a5', {opacity: 0, duration: 0.4, delay: 2.9, ease: "power1.out"})
    gsap.from('#a6', {opacity: 0, duration: 1, delay: 3.2, y: 100,  ease: "power4.out"})
    gsap.from('#a7', {opacity: 0, duration: 1, delay: 3.7, y: 100,  ease: "power4.out"})
    gsap.from('#a8', {opacity: 0, duration: 1, delay: 4.5, y: 100,  ease: "power2.out"})
    gsap.from('#a9', {opacity: 0, duration: 1, delay: 5.2, y: 100,  ease: "power2.out"})
    gsap.from('#a10', {opacity: 0, duration: 1, delay: 6.2, y: 100,  ease: "power1.out"})
    gsap.from('#t1a11', {opacity: 0, duration: 1, delay: 6.9, y: 40,  ease: "power3.out"})
    gsap.from('#t1a11-vl', {opacity: 0, duration: 1, delay: 6.9, scaleY:0,  ease: "power3.out"})
    gsap.from('#t2a12', {opacity: 0, duration: 1, delay: 7.4, x: -60,  ease: "power3.out"})
    gsap.from('#t2a12-hl', {opacity: 0, duration: 1, delay: 7.4, scaleX:0,  ease: "power3.out"})
    gsap.from('#t3a13', {opacity: 0, duration: 1, delay: 8.4, y: 40,  ease: "power3.out"})
    gsap.from('#t3a13-vl', {opacity: 0, duration: 1, delay: 8.4, scaleY:0,  ease: "power3.out"})
  }
}
</script>

<style>
body{
  background-color: black;
}
.tx, .tx div{
  font-size: 17px;
  line-height: 1em;
  transform-origin: top left;
  transform: skew(0deg, 3deg);
}
.vl{
  opacity: 0.1;
  width:2px;
  height: 330px;
  max-width: 2px;
  max-height: 300px;
}
.red{
  color: rgb(216, 57, 89);
}
.red-ot{
  background: rgba(255, 2, 2, 0.2);
}
.green{
  color: aquamarine;
}
.green-ot{
  background: rgba(2, 255, 158, 0.2);
}
.yellow{
  color: rgb(253, 255, 127);
}
.yellow-ot{
  background: rgba(255, 238, 2, 0.2);
}
.hl{
  opacity: 0.1;
  width:270px;
  height: 2px;
  max-width: 270px;
  max-height: 2px;
  transform: skew(0deg, 5.5deg);
}
.anim img, .anim div{
  opacity: 1;
  /* max-width: 500px; */
  position: absolute;
  margin-top:15%;
}
.anim{
  height: 500px;
  display: flex;
  justify-content: center;
}
#app {
  height: 100vh;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
