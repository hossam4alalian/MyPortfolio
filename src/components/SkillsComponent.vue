<template>
    <div class="skills">
      <h2>My Skills & Certifications</h2>

      <div class="skill-group">
          <h3>Languages</h3>
          <ul>
              <li v-for="lang in skills.languages" :key="lang">{{ lang }}</li>
          </ul>
      </div>

      <div class="skill-group">
          <h3>Frameworks & Libraries</h3>
          <ul>
              <li v-for="fw in skills.frameworks" :key="fw">{{ fw }}</li>
          </ul>
      </div>

      <div class="skill-group">
          <h3>Tools & Platforms</h3>
          <ul>
              <li v-for="tool in skills.tools" :key="tool">{{ tool }}</li>
          </ul>
      </div>

      <div class="skill-group">
          <h3>Certifications</h3>
          <ul class="certifications">
              <li v-for="item in skills.certifications" :key="item">{{ item }}</li>
          </ul>
      </div>
    </div>
</template>
  
<script>
  export default {
    name: "SkillsComponent",
    data() {
      return {
        skills: {
          languages: [
            "Java", "JavaScript", "TypeScript", "HTML", "CSS",
            "C#", "PHP", "SQL", "YAML", "JSON"
          ],
          frameworks: [
            "Vue.js", "Vue", "React", "Spring", "REST", "Junit"
          ],
          tools: [
            ".Net", "Delphi", "Git", "SVN"
          ],
          certifications: [
            "Continuing education in the form if a fourth technical year, focus: information technology.",
            "MTA: Introduction till programming using JAVA.",
            "Starta eget utbildning - Nyföretagcentrum",
            "Digital information security training for all (Disa)."
          ]
        }
      };
    }
  };
</script>
  
<style scoped>
  .skills {
    padding: 1.5625rem;
    margin-top: 1.875rem;
    border-bottom: 0.125rem solid #dfdada;
  }

  .skill-group {
    margin-bottom: 1.5625rem;
  }

  .skill-group h3 {
    font-size: 1.5rem;
    margin-bottom: 0.625rem;
  }

  .skill-group ul {
    list-style: none;
    padding: 0;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.75rem;
  }

  .certifications {
    flex-direction: column;
  }

  .skill-group li {
    padding: 0.5rem 0.9375rem;
    border-radius: 0.375rem;
    font-size: 1rem;
    transition: 0.2s;
  }

  @media (max-width: 37.5rem) {
    .skills {
      width: 90%;
      padding: 1.25rem;
    }

    .skills h2 {
      font-size: 1.8rem;
    }

    .skill-group h3 {
      font-size: 1.3rem;
    }

    .skill-group li {
      font-size: 0.95rem;
      padding: 0.4375rem 0.75rem;
    }
  }
</style>
  