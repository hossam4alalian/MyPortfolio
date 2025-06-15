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
          },
          {
            title: "Task Manager (Work in progress)",
            description: "A task manger website.",
            link: ""
          }
        ]
      };
    }
  };
</script>
  
<style scoped>
    .projects {
        padding: 1.875rem 1.875rem 3.75rem; 
        margin-top: 1.5625rem; 
        border-bottom: 0.125rem solid #dfdada; 
    }

    .project-list {
        display: flex;
        flex-wrap: wrap;
        gap: 1.25rem; 
        justify-content: center;
    }

    .project-card {
        background: white;
        padding: 1.25rem; 
        border-radius: 0.625rem; 
        width: 100%;
        max-width: 16.875rem; 
        box-shadow: 0 0.375rem 1.125rem rgba(0, 0, 0, 0.1); 
        transition: transform 0.2s ease;
    }

    .project-card:hover {
        transform: translateY(-0.3125rem);  
    }

    .project-card h3 {
        margin-top: 0;
        font-size: 1.3rem;
        color: #333;
        padding-left: 0.625rem;
        text-align: left;
    }

    .project-card p {
        font-size: 1rem; 
        color: #555;
        margin-bottom: 0.9375rem; 
        text-align: left;
        padding: 10px;
    }

    .project-card a {
        text-decoration: none;
        color: white;
        background-color: #ff416c;
        padding: 0.5rem 0.75rem; 
        border-radius: 0.375rem; 
        font-weight: 500;
        transition: background 0.3s;
    }

    .project-card a:hover {
        background-color: #e1355c;
    }

    .view-projects {
        padding: 0.625rem; 
        text-align: left;
    }
</style>
  