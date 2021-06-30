<template>
  <div>
    <div class="background"></div>
    <div class="blurb-wrapper blurb-item">
      <p class="blurb-intro blurb-item">
        Welcome to my little corner of the web. I am a curious person motivated
        by compassion, social justice, and human connection.
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
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-image: url('@/assets/images/smoke.gif');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}

.blurb-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  align-content: center;
  mix-blend-mode: luminosity;
  margin-top: 5vw;
}

.blurb-item {
  text-align: center;
}

.blurb-intro {
  font-family: Neue Haas Unica W1G;
  font-style: normal;
  font-weight: 700;
  font-size: 54px;
  line-height: 140.62%;
  color: #efe7e0;
  max-width: 900px;
}

.instruction {
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: bold;
  font-size: 48px;
  line-height: 90.12%;
  color: #73688a;
}
</style>
