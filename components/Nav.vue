<template>
  <nav
    :class="{
      sticky: scrollY > 700,
    }"
  >
    <div>
      <div class="nav-flex">
        <h1 class="nav-item">Skylar Soehl-Gutierrez</h1>
        <div class="nav-item link-flex">
          <p>item 1</p>
          <p>item 2</p>
          <p>{{ scrollY }}</p>
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
  padding-top: 3vw;
  padding-left: 3vw;
  padding-right: 3vw;
  pointer-events: auto;
  color: #efe7e0;
  transition: 100ms;
}

.sticky {
  position: fixed;
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
