<template>
    <div class="skills">
      <h2>My Skills</h2>

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
          <h3>Other</h3>
          <ul>
              <li v-for="item in skills.other" :key="item">{{ item }}</li>
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
          other: [
            "Office Package"
          ]
        }
      };
    }
  };
</script>
  
<style scoped>
  .skills {
    background: white;
    padding: 25px;
    border-radius: 12px;
    box-shadow: 0px 6px 18px rgba(0, 0, 0, 0.1);
    text-align: center;
    margin-top: 30px;
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
  }
  
  .skills h2 {
    color: #ff416c;
    font-size: 2rem;
    margin-bottom: 20px;
    text-transform: uppercase;
  }
  
  .skill-group {
    margin-bottom: 25px;
  }
  
  .skill-group h3 {
    font-size: 1.5rem;
    color: #444;
    margin-bottom: 10px;
    text-decoration: underline;
  }
  
  .skill-group ul {
    list-style: none;
    padding: 0;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 12px;
  }
  
  .skill-group li {
    background-color: #f1f1f1;
    padding: 8px 15px;
    border-radius: 6px;
    font-weight: 600;
    font-size: 1rem;
    transition: 0.2s;
  }
  
  @media (max-width: 600px) {
    .skills {
      width: 90%;
      padding: 20px;
    }
  
    .skills h2 {
      font-size: 1.8rem;
    }
  
    .skill-group h3 {
      font-size: 1.3rem;
    }
  
    .skill-group li {
      font-size: 0.95rem;
      padding: 7px 12px;
    }
  }
</style>
  