<template>
  <div class="project-container">
    <ProjectLink class="project-link" name="Payyo" url="/payyo" />
    <ProjectLink
      class="project-link"
      name="The Climate Crisis is Racist"
      url="/tccir"
    />
    <ProjectLink
      class="project-link"
      name="Global Resilience Institute"
      url="/gri"
    />
    <ProjectLink
      class="project-link"
      name="Interventions"
      url="/interventions"
    />
    <ProjectLink class="project-link" name="Butter" url="/butter" />
  </div>
</template>

<script>
export default {}
</script>

<style>
.project-container {
  position: relative;
  padding-left: 5.2vw;
  padding-right: 5.2vw;
}

.project-link {
  position: relative;
  display: flex;
  width: 100%;
  height: auto;
  text-align: left;
  overflow: hidden;
  margin: 2rem 0;
}

@media only screen and (max-width: 770px) {
  .project-link {
    text-align: center;
    justify-content: center;
  }
}
</style>
