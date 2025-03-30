<template>
  <div class="about-me">
      <h2>About Me</h2>
      <h3>Welcome to My portfolio!</h3>
      <p class="about-my-self">
          I'm a positive and social developer who loves meeting new people and sharing good vibes 😄
          Whether I'm working solo or collaborating in a team, I'm always up for a challenge and eager to grow.
          <br/>
          Outside of code, you'll find me kicking a football ⚽, or gaming and chatting with people from all over the world 🎮🌍
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

  .about-my-self {
    padding-bottom: 2em;
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
  