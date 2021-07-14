<template>
  <nav
    :class="{
      sticky: scrollY > 900,
    }"
  >
    <div class="nav-container">
      <div class="nav-flex">
        <h1 class="nav-item">
          <NuxtLink
            class="nav-link"
            :class="scrollY > 900 ? 'nav-link-sticky' : 'nav-link-fixed'"
            to="/"
          >
            Skylar Soehl<span class="name-italic">-Gutierrez</span></NuxtLink
          >
        </h1>
        <div class="nav-item link-flex">
          <NuxtLink
            class="nav-link"
            :class="scrollY > 700 ? 'nav-link-sticky' : 'nav-link-fixed'"
            to="/"
            >Fun</NuxtLink
          >
          <NuxtLink
            class="nav-link"
            :class="scrollY > 700 ? 'nav-link-sticky' : 'nav-link-fixed'"
            to="/"
            >About</NuxtLink
          >
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
  position: absolute;
  width: 100%;
  padding-top: 30px;
  z-index: 2;
  pointer-events: auto;
}

.nav-container {
  padding-left: 5.2vw;
  padding-right: 5.2vw;
}

h1 {
  font-family: Neue Haas Unica W1G;
  font-weight: bold;
  font-size: 36px;
  line-height: 47px;
}

.nav-link {
  text-decoration: none;
  transition: 800ms;
}

.nav-link-sticky {
  color: black;
}

.nav-link-fixed {
  color: #efe7e0;
}

.nav-link:hover {
  transition: 800ms;
  color: #f83c22;
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
  width: 100vw;
  transition: 200ms;
  background-color: #efe7e0;
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

.link-flex > * {
  margin-right: 100px;
}
</style>
