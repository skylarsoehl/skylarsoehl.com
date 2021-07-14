<template>
  <div class="container">
    <div class="back-link">
      <div class="back-arrow">
        <svg
          width="63"
          height="24"
          viewBox="0 0 63 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M0.939335 10.9393C0.35355 11.5251 0.35355 12.4749 0.939335 13.0607L10.4853 22.6066C11.0711 23.1924 12.0208 23.1924 12.6066 22.6066C13.1924 22.0208 13.1924 21.0711 12.6066 20.4853L4.12132 12L12.6066 3.51472C13.1924 2.92893 13.1924 1.97919 12.6066 1.3934C12.0208 0.807611 11.0711 0.807611 10.4853 1.3934L0.939335 10.9393ZM63 10.5L2 10.5V13.5L63 13.5V10.5Z"
            fill="black"
          />
        </svg>
      </div>
      <p class="back-text">Back</p>
    </div>
    <div class="landing">
      <div class="background">
        <img
          src="@/assets/images/payyo/Ifugao-elders-in-tradtional-dress.jpg"
          alt=""
        />
      </div>
      <div class="text-container">
        <h1 class="project-title">Payyo</h1>
      </div>
      <div class="bottom-link">
        <div class="link-container">
          <p class="bottom-link-text">see more</p>
          <svg
            class="icon-arrow-down"
            width="18px"
            height="7px"
            viewBox="0 0 18 7"
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
          >
            <g stroke="none" stroke-width="1" fill-rule="evenodd">
              <g
                transform="translate(-756.000000, -107.000000)"
                fill-rule="nonzero"
              >
                <path
                  d="M765,113.3 C764.9,113.3 764.7,113.3 764.6,113.2 L756,108.5 L756.8,107 L765,111.5 L773.1,107 L773.9,108.5 L765.4,113.2 C765.3,113.3 765.1,113.3 765,113.3 Z"
                ></path>
              </g>
            </g>
          </svg>
        </div>
      </div>
    </div>
    <div class="overview">
      <div class="description">
        <p>
          This project is from my Design Synthesis class, where we each chose a
          UNESCO World Heritage site for which we created a brand identity and
          various types of collateral. I chose the The Rice Terraces of the
          Philippine Cordilleras because I was inspired by the site’s story of
          colonial resistance and wanted to design a brand that paid hommeage to
          the native people of the Ifugao province. "Payyo" is name of the land
          in the native language.
        </p>
      </div>
      <div class="scope">
        <h2>Project Scope</h2>
        <div class="year category">
          <p class="title">year</p>
          <p class="category-value">2021</p>
        </div>
        <div class="role category">
          <p class="title">role</p>
          <p class="category-value">Designer</p>
        </div>
        <div class="collaborators category">
          <p class="title">collaborators</p>
        </div>
        <div class="disciplines category">
          <p class="title">disciplines</p>
          <ul></ul>
        </div>
      </div>
    </div>
    <div class="curtain-img">
      <img src="@/assets/images/payyo/rice-terraces-1.jpg" alt="" />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.container {
  margin-bottom: 8rem;
}
.landing {
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  width: 100%;
  height: 100vh;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
}

.back-link {
  position: fixed;
  z-index: 2;
  display: flex;
  align-items: center;
  margin: 2rem 5rem;
}

.back-arrow {
  fill: black;
  margin-right: 20px;
  width: 61px;
  height: 20px;
}

.back-text {
  font-size: 24px;
}

.background {
  position: absolute;
  display: block;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
}

.background > img {
  width: 100%;
  height: 100%;
  -o-object-fit: cover;
  object-fit: cover;
}

.text-container {
  position: relative;
  padding: 0 var(--lateral-space);
  margin-top: 8rem;
}

.project-title {
  font-size: 10vw;
  line-height: 7.5vw;
  color: #c7bfb8;
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: normal;
}

.bottom-link {
  position: absolute;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  width: 100%;
  bottom: 75px;
  left: 0;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
}

.link-container {
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  text-align: center;
}

.bottom-link-text {
  font-family: Neue Haas Unica W1G;
  font-weight: bold;
  font-size: 30px;
  color: #fff;
}

.icon-arrow-down {
  width: 20px;
  height: 20px;
  fill: #fff;
}

.overview {
  margin-bottom: 0;
  display: flex;
  position: relative;
}

.description {
  padding: 110px 10vw;
  font-family: Neue Haas Unica W1G;
  font-size: 36px;
  line-height: 140.62%;
  width: 80%;
}

.scope {
  width: 20%;
  padding: 110px 10vw;
  font-size: 18px;
  background: #efe7e0;
}

.category > .title {
  color: #aa9c8e;
  font-size: 16px;
  font-variant: small-caps;
  font-weight: 600;
}

.curtain-img {
  height: 650px;
  width: 100%;
}

.curtain-img > img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
