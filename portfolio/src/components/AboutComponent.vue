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
        <h3>EagleVision:</h3>
        <p>
            We provide custom web and app solutions for businesses and develop our own tech products alongside consultancy services.
        </p>
    </div>
  </template>
  
  <script>
  export default {
    name: "AboutMeComponent"
  };
  </script>
  
<style scoped>
  /* About Me Section */
  .about-me {
    background: white;
    padding: 0px;
    border-radius: 12px;
    box-shadow: 0px 6px 18px rgba(0, 0, 0, 0.1);
    text-align: center;
    margin-top: 30px;
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
  }
  
  /* Heading */
  .about-me h2 {
    color: #ff416c;
    font-size: 2rem;
    text-transform: uppercase;
    margin-bottom: 15px;
  }
  
  /* Paragraph */
  .about-me p {
    font-size: 1.2rem;
    color: #333;
    line-height: 1.6;
  }
  
  /* Responsive */
  @media (max-width: 600px) {
    .about-me {
      width: 90%;
      padding: 20px;
    }
  
    .about-me h2 {
      font-size: 1.8rem;
    }
  
    .about-me p {
      font-size: 1rem;
    }
  }
</style>
  