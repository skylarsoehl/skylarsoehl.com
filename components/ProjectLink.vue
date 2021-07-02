<template>
  <div>
    <NuxtLink class="project-link blur out shake" :to="`project${url}`">{{
      name
    }}</NuxtLink>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: '',
    },
    url: {
      type: String,
      default: '/',
    },
  },
  mounted() {
    // append textshadow class to HTML node if supported (Modernizr will do the same)
    if (document.createElement('detect').style.textShadow === '') {
      document.getElementsByTagName('html')[0].className += ' textshadow'
    }
  },
}
</script>

<style>
.project-link {
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: normal;
  font-size: 96px;
  line-height: 109.63%;
}

.blur {
  text-decoration: none;
  color: black;
}

.textshadow .blur,
.textshadow .blur:hover,
.textshadow .blur:focus {
  text-decoration: none;
  color: rgba(0, 0, 0, 0);
  outline: 0 none;
  -webkit-transition: 400ms ease 100ms;
  -moz-transition: 400ms ease 100ms;
  transition: 400ms ease 100ms;
}

/* no blur */
.textshadow .blur.out,
.textshadow .blur:hover,
.textshadow .blur:focus {
  text-shadow: 0 0 0 black;
}

/* full blur */
.textshadow .blur,
.textshadow .blur.out:hover,
.textshadow .blur.out:focus {
  text-shadow: 0 0 4px #f83c22;
}

.project-link:hover {
  animation: shake 0.1s infinite;
}

@keyframes shake {
  0% {
    transform: translate(0.25px, 0.25px) rotate(0deg);
  }
  10% {
    transform: translate(-0.25px, -0.5px) rotate(0deg);
  }
  20% {
    transform: translate(-0.75px, 0px) rotate(0deg);
  }
  30% {
    transform: translate(0.75px, 0.5px) rotate(0deg);
  }
  40% {
    transform: translate(0.25px, -0.25px) rotate(0deg);
  }
  50% {
    transform: translate(-0.25px, 0.5px) rotate(0deg);
  }
  60% {
    transform: translate(-0.75px, 0.25px) rotate(0deg);
  }
  70% {
    transform: translate(0.75px, 0.25px) rotate(0deg);
  }
  80% {
    transform: translate(-0.25px, -0.25px) rotate(0deg);
  }
  90% {
    transform: translate(0.25px, 0.5px) rotate(0deg);
  }
  100% {
    transform: translate(0.25px, -0.75px) rotate(0deg);
  }
}
</style>
