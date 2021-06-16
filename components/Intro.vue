<template>
  <div>
    <div class="background"></div>
    <div class="blurb-wrapper">
      <p class="blurb-text">
        Welcome to my little corner of the web. I am a curious person driven by
        compassion, social justice, and adventure.
      </p>
      <p class="instruction">Scroll to view my work</p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.background {
  width: 100%;
  height: 100vh;
  background-image: url('@/assets/images/smoke.gif');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  overflow: hidden;
}

.blurb-wrapper {
  position: fixed;
  top: 0;
  left: 0;
  pointer-events: none;
  mix-blend-mode: luminosity;
}

.blurb-text {
  font-family: Neue Haas Unica W1G;
  font-style: normal;
  font-weight: normal;
  font-size: 54px;
  line-height: 140.62%;
  /* or 90px */

  position: relative;
  display: block;
  width: auto;
  margin: 32vh 12vw 0 8vw;
  padding-right: 24vw;
  color: #efe7e0;
}

.instruction {
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: bold;
  font-size: 48px;
  line-height: 90.12%;
  color: #73688a;
  text-align: center;
  margin: 10vh 0 0;
}
</style>
