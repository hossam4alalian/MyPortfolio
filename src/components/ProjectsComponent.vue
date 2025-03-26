<template>
    <div class="projects">
        <h2>My Projects</h2>
        <div class="project-list">
            <div class="project-card" v-for="project in projects" :key="project.title">
                <h3>{{ project.title }}</h3>
                <p>{{ project.description }}</p>
                <div class="view-projects">
                    <a :href="project.link" target="_blank" v-if="project.link">View Project</a>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>
  export default {
    name: "ProjectsComponent",
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
  .projects {
    background: white;
    padding: 30px 30px 60px;
    text-align: center;
    margin-top: 30px;
    max-width: 900px;
    margin-left: auto;
    margin-right: auto;
    border-bottom: 2px solid #dfdada;
  }
  
  .projects h2 {
    color: #ff416c;
    font-size: 2rem;
    margin-bottom: 25px;
    text-transform: uppercase;
  }
  
  .project-list {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
  }
  
  .project-card {
    background: white;
    padding: 20px;
    border-radius: 10px;
    width: 100%;
    max-width: 270px;
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s ease;
  }
  
  .project-card:hover {
    transform: translateY(-5px);
  }
  
  .project-card h3 {
    margin-top: 0px;
    font-size: 1.3rem;
    color: #333;
  }
  
  .project-card p {
    font-size: 1rem;
    color: #555;
    margin-bottom: 15px;
  }
  
  .project-card a {
    text-decoration: none;
    color: white;
    background-color: #ff416c;
    padding: 8px 12px;
    border-radius: 6px;
    font-weight: 500;
    transition: background 0.3s;
  }
  
  .project-card a:hover {
    background-color: #e1355c;
  }

  .view-projects {
    padding: 10px;
  }
</style>
  