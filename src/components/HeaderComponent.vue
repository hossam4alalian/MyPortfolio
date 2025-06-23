<template>
  <div class="header">
      <h1>Sam Alalian</h1>
      <h2>Software Engineer</h2>
  </div>
</template>

<script>
  export default {
    name: 'HeaderComponent',
    props: {
    }
  }
</script>

<style scoped>
  .header {
    width: 90%;
    margin: auto;
    max-width: 42rem;
    background: linear-gradient(to right, #ff4b2b, #ff416c);
    color: white;
    padding: 25px;
    border-radius: 15px;
    animation: fadeInSlide 0.8s ease-out;
    border-bottom: 2px solid #dfdada;
  }

  .header h1 {
    font-size: 2.8rem;
    font-weight: bold;
    margin: 0;
    text-transform: uppercase;
    letter-spacing: 1.8px;
  }

  .header h2 {
    font-size: 1.3rem;
    font-weight: 400;
    margin-top: 5px;
    opacity: 0.9;
    color: white;
  }

  @media (max-width: 37.5rem) {
    .header {
      width: unset;
    }

    .header h1 {
      font-size: 2.2rem;
      padding-bottom: 0.5em;
    }

    .header h2 {
      font-size: 1.1rem;
    }
  }

  @keyframes fadeInSlide {
    from {
      opacity: 0;
      transform: translateY(-20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
</style>


  