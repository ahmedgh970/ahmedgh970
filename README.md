# 👋 Hi, I’m Ahmed

💻 **Computer Vision Engineer** at Ecole Polytechnique (l'X), France.

📚 **Background**: Hailing from STEM background with validated experience in applying machine learning and computer vision to industrial applications. 

🌱 **Current Focus**: Currently designing and implementing diffusion models, with a focus on conditional image generation and traffic simulation.

🤝 **Collaboration**: Open to collaborations on impactful projects, especially those in healthcare and other high-impact fields.




# 👋 Hi, I’m <span id="dynamic-name">Ahmed</span>

Welcome to my GitHub profile! I'm a **Computer Vision Engineer** with expertise in generative AI. Explore my repositories to see what I’ve been working on recently.

---

## 🛠️ **Technologies I Work With**
- **Programming**: Python
- **Frameworks**: TensorFlow, PyTorch
- **Tools**: VS-Code, PyCharm, Docker, Singularity, Git, CI/CD, AWS, GCP
- **OS**: Linux
- **AI Expertise**:
  - GenAI: motion forecasting and image synthesis
  - Learning-based image and video compression
  - Anomaly detection and segmentation

---

## 📈 **GitHub Stats**
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YourGitHubUsername&show_icons=true&theme=radical" alt="GitHub Stats">
</p>

---

## 📫 **Get in Touch**
- **Email**: [ghorbel.ahmd@gmail.com](mailto:ghorbel.ahmd@gmail.com)
- **LinkedIn**: [linkedin.com/in/ahmed-ghorbel97/](#)

---

<script>
  const name = "Ahmed";
  const container = document.getElementById("dynamic-name");

  let index = 0;

  function typeEffect() {
      if (index < name.length) {
          container.innerHTML += name[index];
          index++;
          setTimeout(typeEffect, 150); // Adjust speed here
      } else {
          addCursorEffect();
      }
  }

  function addCursorEffect() {
      const cursor = document.createElement("span");
      cursor.innerText = "|";
      cursor.style.animation = "blink 0.7s steps(2, start) infinite";
      container.appendChild(cursor);
  }

  typeEffect();
</script>

<style>
  #dynamic-name::after {
      content: '';
      display: inline-block;
  }

  @keyframes blink {
      50% {
          opacity: 0;
      }
  }
</style>
