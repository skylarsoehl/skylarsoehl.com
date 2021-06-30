<template>
  <div>
    <Nav />
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family: Neue Haas Unica W1G, 'Source Sans Pro', -apple-system,
    BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  margin: 0;
  padding-top: 50px;
  padding-left: 5.2vw;
  padding-right: 5.2vw;
}

header {
  position: fixed;
  width: 100%;

  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  align-items: center;

  z-index: 2;
}
.serif {
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: bold;
  font-size: 38px;
  line-height: 47px;
}

.slide-bottom-enter-active,
.slide-bottom-leave-active {
  transition: opacity 0.25s ease-in-out, transform 0.25s ease-in-out;
}
.slide-bottom-enter,
.slide-bottom-leave-to {
  opacity: 0;
  transform: translate3d(0, 15px, 0);
}
</style>
