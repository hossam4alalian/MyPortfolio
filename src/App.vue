<template>
  <HeaderComponent />
  <AboutComponent />
  <SkillsComponent />
  <ContactComponent />
</template>

<script>
  import AboutComponent from './components/AboutComponent.vue';
  import ContactComponent from './components/ContactComponent.vue';
  import HeaderComponent from './components/HeaderComponent.vue'
  import SkillsComponent from './components/SkillsComponent.vue';

  export default {
    name: 'App',
    components: {
      HeaderComponent,
      SkillsComponent,
      AboutComponent,
      ContactComponent
    }
  }
</script>

<style>
  #app {
    font-family: "Poppins", Avenir, Helvetica, Arial, sans-serif;
    text-align: center;
    color: #333;
    margin-top: 10px;
    background: #f8f9fa;
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

