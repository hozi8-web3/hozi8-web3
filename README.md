<div align="center">
  
  <!-- Animated Typing Header with Gradient -->
  <div align="center">
    <h1 style="background: linear-gradient(45deg, #00ff00, #00ffff, #ff00ff, #00ff00); background-size: 300% 300%; animation: gradient 3s ease infinite; -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; font-size: 2.5em; font-weight: bold; margin: 20px 0;">
      <span id="typing-text"></span>
    </h1>
  </div>

  <!-- CSS for Gradient Animation -->
  <style>
    @keyframes gradient {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    
    .glow-text {
      text-shadow: 0 0 10px #00ff00, 0 0 20px #00ff00, 0 0 30px #00ff00;
      animation: glow 2s ease-in-out infinite alternate;
    }
    
    @keyframes glow {
      from { text-shadow: 0 0 10px #00ff00, 0 0 20px #00ff00, 0 0 30px #00ff00; }
      to { text-shadow: 0 0 20px #00ff00, 0 0 30px #00ff00, 0 0 40px #00ff00; }
    }
    
    .floating {
      animation: floating 3s ease-in-out infinite;
    }
    
    @keyframes floating {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0px); }
    }
  </style>

  <!-- JavaScript for Typing Animation -->
  <script>
    const texts = [
      "Hi there 👋 I'm HOZAIFA ALI",
      "aka HOZI 💻",
      "Web3 Developer | Backend Wizard | AI Enthusiast",
      "Discord Moderator & Bot Developer 🤖",
      "Always building cool private projects 🚀"
    ];
    
    let textIndex = 0;
    let charIndex = 0;
    let isDeleting = false;
    
    function typeText() {
      const currentText = texts[textIndex];
      
      if (isDeleting) {
        document.getElementById('typing-text').textContent = currentText.substring(0, charIndex - 1);
        charIndex--;
      } else {
        document.getElementById('typing-text').textContent = currentText.substring(0, charIndex + 1);
        charIndex++;
      }
      
      if (!isDeleting && charIndex === currentText.length) {
        setTimeout(() => isDeleting = true, 2000);
      } else if (isDeleting && charIndex === 0) {
        isDeleting = false;
        textIndex = (textIndex + 1) % texts.length;
      }
      
      const speed = isDeleting ? 100 : 150;
      setTimeout(typeText, speed);
    }
    
    // Start typing animation when page loads
    window.onload = typeText;
  </script>

  <!-- Profile Views Counter -->
  <p align="center" class="floating">
    <img src="https://komarev.com/ghpvc/?username=hozi8-web3&style=flat-square&color=00ff00&label=PROFILE+VIEWS" alt="Profile Views" />
  </p>

  <!-- Social Badges -->
  <p align="center" class="floating">
    <a href="https://github.com/hozi8-web3?tab=followers">
      <img alt="followers" title="Follow me on Github" src="https://custom-icon-badges.demolab.com/github/followers/hozi8-web3?color=00ff00&labelColor=1b1b1b&style=for-the-badge&logo=person-add&label=FOLLOWERS&logoColor=white"/>
    </a>
  </p>

  <!-- Cool Divider -->
  <div align="center">
    <img src="https://github.com/hozi8-web3/hozi8-web3/blob/main/assets/divider.svg" alt="divider" width="100%"/>
  </div>

  <!-- GitHub Stats -->
  <div align="center" class="floating">
    <img src="https://github-readme-stats.vercel.app/api?username=hozi8-web3&show_icons=true&theme=radical&hide_border=true&bg_color=0d1117&title_color=00ff00&text_color=ffffff&icon_color=00ff00&border_radius=10" alt="GitHub Stats" />
  </div>

  <!-- GitHub Streak Stats -->
  <div align="center" class="floating">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=hozi8-web3&theme=radical&hide_border=true&background=0d1117&stroke=00ff00&ring=00ff00&fire=00ff00&currStreakNum=ffffff&sideNums=ffffff&currStreakLabel=00ff00&sideLabels=00ff00&dates=ffffff" alt="GitHub Streak Stats" />
  </div>

  <!-- GitHub Trophies -->
  <div align="center" class="floating">
    <img src="https://github-profile-trophy.vercel.app/?username=hozi8-web3&theme=radical&no-frame=true&no-bg=false&margin-w=4&margin-h=4&row=1&column=6" alt="GitHub Trophies" />
  </div>

  <!-- Contribution Graph with Activity -->
  <div align="center" class="floating">
    <h2 style="color: #00ff00; margin: 20px 0;">📊 Contribution Activity</h2>
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=hozi8-web3&theme=react-dark&hide_border=true&area=true&color=00ff00&line=00ff00&point=ffffff&area_color=00ff00&area_alpha=0.3" alt="Contribution Graph" />
  </div>

  <!-- Skills Section -->
  <h2 align="center" class="glow-text">🛠️ Skills & Technologies</h2>
  <div align="center" class="floating">
    <img src="https://skillicons.dev/icons?i=js,ts,py,solidity,nodejs,express,mongodb,react,nextjs,github,git,linux,docker&theme=dark&perline=7" alt="Skills" />
  </div>

  <!-- Cool Divider -->
  <div align="center">
    <img src="https://github.com/hozi8-web3/hozi8-web3/blob/main/assets/divider.svg" alt="divider" width="100%"/>
  </div>

  <!-- Private Projects Section -->
  <h2 align="center" class="glow-text">🚧 Private Projects</h2>
  <div align="center" class="floating">
    <p>
      <em>Many of my contributions are in private repositories and don't show publicly, but rest assured - there's always something cool being built behind the scenes! 🔒✨</em>
    </p>
    <p>
      <strong>Current Focus:</strong> Web3 DApps, AI-powered backend services, and scalable microservices architecture
    </p>
  </div>

  <!-- Discord Experience Section -->
  <h2 align="center" class="glow-text">🤖 Discord Experience</h2>
  <div align="center" class="floating">
    <p>
      <em>Experienced Discord moderator and bot developer! I create custom Discord bots with advanced features including:</em>
    </p>
    <p>
      <strong>Bot Features:</strong> Moderation tools, custom commands, music integration, welcome systems, and automated responses
    </p>
    <p>
      <strong>Moderation Skills:</strong> Community management, rule enforcement, event organization, and user engagement
    </p>
  </div>

  <!-- Cool Divider -->
  <div align="center">
    <img src="https://github.com/hozi8-web3/hozi8-web3/blob/main/assets/divider.svg" alt="divider" width="100%"/>
  </div>

  <!-- Connect Section -->
  <h2 align="center" class="glow-text">🌐 Connect with Me</h2>
  <div align="center" class="floating">
    <a href="https://linkedin.com/in/hozaifa-ali" target="_blank">
      <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&color=00ff00" alt="LinkedIn" />
    </a>
    <a href="https://twitter.com/hozi8_web3" target="_blank">
      <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white&color=00ff00" alt="Twitter" />
    </a>
    <a href="mailto:hozaifa.ali@example.com">
      <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white&color=00ff00" alt="Email" />
    </a>
    <a href="https://github.com/hozi8-web3" target="_blank">
      <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white&color=00ff00" alt="GitHub" />
    </a>
    <a href="https://discord.com/users/your-discord-id" target="_blank">
      <img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white&color=00ff00" alt="Discord" />
    </a>
  </div>

  <!-- Cool Divider -->
  <div align="center">
    <img src="https://github.com/hozi8-web3/hozi8-web3/blob/main/assets/divider.svg" alt="divider" width="100%"/>
  </div>

  <!-- Quote Section -->
  <h2 align="center" class="glow-text">💡 Quote of the Day</h2>
  <div align="center" class="floating">
    <blockquote style="border-left: 4px solid #00ff00; padding-left: 20px; font-style: italic;">
      <em>"The best way to predict the future is to implement it."</em>
      <br>
      <strong>- David Heinemeier Hansson</strong>
    </blockquote>
  </div>

  <!-- Cool Divider -->
  <div align="center">
    <img src="https://github.com/hozi8-web3/hozi8-web3/blob/main/assets/divider.svg" alt="divider" width="100%"/>
  </div>

  <!-- Footer -->
  <div align="center" class="floating">
    <p>
      <em>Thanks for visiting! Feel free to reach out if you want to collaborate on something awesome! 🚀</em>
    </p>
  </div>

</div>
