<template>
  <ContainerComponent>
    <HeaderComponent />
    <AboutComponent />
    <SkillsComponent />
    <ProjectsComponent />
    <ContactComponent />
  </ContainerComponent>
</template>

<script>
  import AboutComponent from './components/AboutComponent.vue';
  import ContactComponent from './components/ContactComponent.vue';
  import ContainerComponent from './components/ContainerComponent.vue';
  import HeaderComponent from './components/HeaderComponent.vue'
  import ProjectsComponent from './components/ProjectsComponent.vue';
  import SkillsComponent from './components/SkillsComponent.vue';

  export default {
    name: 'App',
    components: {
      HeaderComponent,
      SkillsComponent,
      AboutComponent,
      ProjectsComponent,
      ContactComponent,
      ContainerComponent
    }
  }
</script>

<style>
  #app {
    font-family: "Poppins", Avenir, Helvetica, Arial, sans-serif;
    margin-top: 0.625rem;
    padding-bottom: 3.125rem;
  }
</style>

