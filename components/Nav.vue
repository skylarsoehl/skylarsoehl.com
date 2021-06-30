<template>
  <nav
    :class="{
      sticky: scrollY > 700,
    }"
  >
    <div>
      <div class="nav-flex">
        <h1 class="nav-item">
          Skylar Soehl<span class="name-italic">-Gutierrez</span>
        </h1>
        <div class="nav-item link-flex">
          <p>item 1</p>
          <p>item 2</p>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      scrollY: 0,
    }
  },
  mounted() {
    window.addEventListener('scroll', () => {
      this.scrollY = window.scrollY
    })
  },
  transitions: 'slide-bottom',
}
</script>

<style>
nav {
  position: relative;
  z-index: 2;
  width: 100%;
  box-sizing: border-box;
  pointer-events: auto;
  color: #efe7e0;
  transition: 100ms;
}

h1 {
  font-family: Neue Haas Unica W1G;
  font-weight: bold;
  font-size: 38px;
  line-height: 47px;
  color: #efe7e0;
}

.name-italic {
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: bold;
  font-size: 42px;
  line-height: 47px;
}

.sticky {
  position: fixed;
  margin-top: -8rem;
  padding-right: 5.2vw;
  transition: 150ms;
  background-color: blue;
}

.nav-flex {
  display: flex;
  justify-content: space-between;
}

.nav-item {
  flex: 1;
}

.link-flex {
  display: flex;
  justify-content: flex-end;
}

.link-flex > p {
  margin-right: 100px;
}
</style>
