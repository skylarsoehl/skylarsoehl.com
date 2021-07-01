<template>
  <div class="container">
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
    <ProjectLink class="project-link" name="Fubu" url="/fubu" />
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
.container {
  margin-top: 10rem;
  font-size: 32px;
  display: flex;
  flex-direction: column;
}

.project-link {
  margin: 3rem 0;
}
</style>
