<template>
  <div>
    <section class="project-text">
      <h2>Logo</h2>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum.
      </p>
    </section>
    <section class="project-images">
      <img
        class="moodboard"
        src="@/assets/images/payyo/payyo_moodboard.png"
        alt="moodboard showing images of ifugao people, native animals, different rice terraces, indigenous textiles, patterns, and font options"
      />
      <img src="@/assets/images/payyo/week1_logos.jpg" alt="" />
    </section>
  </div>
</template>

<script>
export default {
  layout: 'project',
}
</script>

<style>
section.project-text {
  display: flex;
  align-items: flex-start;
  margin-bottom: 5rem;
}

section.project-text > h2 {
  font-family: Kings Caslon;
  font-style: italic;
  font-weight: normal;
  font-size: 48px;
  line-height: 140.62%;
  margin-right: 80px;
  margin-top: 0;
}

section.project-text > p {
  font-family: Neue Haas Unica W1G;
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 140.62%;
  max-width: 950px;
}

section.project-images {
  display: flex;
  justify-content: space-between;
}

.moodboard {
  max-height: 410px;
}
</style>
