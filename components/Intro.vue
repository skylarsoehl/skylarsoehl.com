<template>
  <div class="container">
    <div class="background"></div>
    <div class="blurb-wrapper">
      <p class="blurb-intro blurb-item">
        Welcome to my little corner of the web. I am a curious person motivated
        by compassion, social justice, and human connection.
      </p>
      <p class="instruction blurb-item">Scroll to view my work</p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  position: relative;
  width: 100%;
  height: 100vh;
}

.background {
  position: absolute;
  width: 100%;
  height: 100vh;
  background-image: url('@/assets/images/home/smoke.gif');
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-position: center;
}

.blurb-wrapper {
  position: relative;
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  align-content: center;
  mix-blend-mode: luminosity;
}

.blurb-item {
  text-align: center;
  padding-top: 7rem;
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

@media only screen and (max-width: 770px) {
  .blurb-wrapper {
    width: 80%;
    margin-left: 5rem;
  }

  .blurb-intro,
  .instruction {
    font-size: 36px;
  }
}

@media only screen and (max-width: 420px) {
  .blurb-wrapper {
    width: 80%;
    margin-left: 36px;
  }

  .blurb-intro,
  .instruction {
    font-size: 28px;
  }
}
</style>
