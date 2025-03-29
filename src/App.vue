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
    text-align: center;
    color: #333;
    margin-top: 10px;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 50px;
  }

  * {
    transition: all 0.3s ease-in-out;
  }
</style>

