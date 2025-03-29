<template>
  <div class="about-me">
      <h2>About Me</h2>
      <h3>Welcome to My portfolio!</h3>
      <p>
          I am 26 years old and grew up in Aleppo in Syria, I moved to Sweden in 2013. I think it is very important to be happy at work, it is interesting and important to work in a competence team to get new challenges and develop, but I can also work by myself.
          <br/>
          I am a person who always tries to be happy and to make everyone around me happy. I always try to be social and get to know new people. Likes to play football, guitar, and computer games to talk to new people around the world.
          <br/>
      </p>
      <h3>EagleVision</h3>
      <p>
          We provide custom web and app solutions for businesses and develop our own tech products alongside consultancy services.
      </p>
  </div>
</template>
  
<script>
  export default {
    name: "AboutComponent"
  };
</script>
  
<style scoped>
  .about-me {
    padding: 2.5rem; 
    margin-top: 1.875rem;  
    border-bottom: 0.125rem solid #dfdada; 
  }

  .about-me p {
    font-size: 1rem;         
    color: #333;
    line-height: 1.6;
  }

  .about-me h3 {
    font-size: 1.5rem;
  }

  @media (max-width: 37.5rem) {
    .about-me {
      padding: 1.25rem;        
    }
  }
</style>
  