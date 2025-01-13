- 👋 Hi, I’m @AchrafELGhazi
- 👀 I’m interested in software development, AI, creative media projects, and community-driven initiatives.
- 🌱 I’m currently a sophomore computer science student,and a part-time software developer at neoCedrus.
- 💞️ I’m looking to collaborate on impactful projects in app development, student engagement platforms, and innovative tech solutions.
- 📫 How to reach me: a.elghazi@aui.ma
- 😄 Pronouns: He/Him
- ⚡ Fun fact: I’m not just a software developer but also a team player who thrives in turning ideas into reality, whether it’s through code or organizing community events !

<!---
AchrafELGhazi/AchrafELGhazi is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
## 🌟 Code Playground

```html
<div style="background: black; color: green; font-family: monospace; overflow: hidden; padding: 20px;">
  <pre id="matrix"></pre>
</div>

<script>
  const matrixEffect = () => {
    const matrixContainer = document.getElementById('matrix');
    const columns = 80;
    const rows = 15;
    const chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZ123456789@#$%^&*()*&^%";
    let matrix = [];

    for (let x = 0; x < columns; x++) {
      matrix[x] = 1;
    }

    const draw = () => {
      matrixContainer.textContent = '';
      for (let i = 0; i < columns; i++) {
        matrixContainer.textContent += chars.charAt(Math.floor(Math.random() * chars.length));
        if (Math.random() > 0.975) {
          matrix[i] = 0;
        }
        matrix[i]++;
      }
      matrixContainer.textContent += '\n';
    };

    setInterval(draw, 100);
  };

  document.addEventListener("DOMContentLoaded", matrixEffect);
</script>
