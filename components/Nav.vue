<template>
  <nav
    :class="{
      sticky: scrollY > screenHeight,
    }"
  >
    <div class="nav-container">
      <div class="nav-flex">
        <h1 class="name nav-item">
          <NuxtLink
            class="link"
            :class="
              scrollY > screenHeight ? 'nav-link-sticky' : 'nav-link-fixed'
            "
            to="/"
          >
            Skylar Soehl<span class="name-italic">-Gutierrez</span></NuxtLink
          >
        </h1>
        <div class="nav-item link-flex">
          <NuxtLink
            class="link nav-link"
            :class="
              scrollY > screenHeight ? 'nav-link-sticky' : 'nav-link-fixed'
            "
            to="/"
            >Fun</NuxtLink
          >
          <NuxtLink
            class="link nav-link"
            :class="
              scrollY > screenHeight ? 'nav-link-sticky' : 'nav-link-fixed'
            "
            to="/"
            >About</NuxtLink
          >
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import NuxtSSRScreenSize from 'nuxt-ssr-screen-size'
export default {
  mixins: [NuxtSSRScreenSize.NuxtSSRScreenSizeMixin],
  data() {
    return {
      scrollY: 0,
      screenHeight: 0,
    }
  },
  mounted() {
    window.addEventListener('scroll', () => {
      this.scrollY = window.scrollY
    })
    this.screenHeight = this.$vssHeight
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

.link {
  text-decoration: none;
  transition: 800ms;
}

.nav-link {
  font-size: 22px;
  font-weight: bold;
}
.nav-link-sticky {
  color: #f83c22;
}

.nav-link-fixed {
  color: #efe7e0;
}

.link:hover {
  transition: 800ms;
  color: #000;
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
  align-items: center;
}

.nav-item {
  flex: 1;
}

.link-flex {
  display: flex;
  justify-content: flex-end;
}

.link-flex > a:first-child {
  margin-right: 100px;
}

@media only screen and (max-width: 770px) {
  h1 {
    font-size: 30px;
  }
  .name-italic {
    font-size: 34px;
  }
  .nav-link {
    font-size: 24px;
  }
  .link-flex > a:first-child {
    margin-right: 50px;
  }
}

@media only screen and (max-width: 420px) {
  h1 {
    font-size: 16px;
  }
  .name-italic {
    font-size: 18px;
  }
  .nav-link {
    font-size: 16px;
  }
  .link-flex > a:first-child {
    margin-right: 50px;
  }
}
</style>
