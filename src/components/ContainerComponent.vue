<template>
    <div class="container">
        <slot />
    </div>
</template>
  
<script>
  export default {
    name: "ContainerComponent",
    data() {
      return {
        projects: [
          {
            title: "Quizy",
            description: "A quiz website for schools and fun.",
            link: "https://quizyhils.com/"
          }
        ]
      };
    }
  };
</script>
  
<style scoped>
    .container {
        background: white;
        text-align: center;
        margin-left: auto;
        margin-right: auto;
        max-width: 70%;
    }

    ::v-deep h2 {
        color: #ff416c;
        font-size: 2rem;
        margin-bottom: 1.25rem;
        text-transform: uppercase;
    }

    @media (max-width: 37.5rem) {
        .container {
            max-width: 90%;
        }
    }
</style>
  