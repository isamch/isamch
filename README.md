<div align="center">
  <!-- Animated Banner -->
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Isam%20Chajia&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32"/>

  <!-- Typing Animation -->
  <p align="center">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&duration=4000&pause=1000&color=2E9EF7&center=true&vCenter=true&width=600&lines=Hi+👋+I'm+Isam+Chajia;Passionate+Web+Developer;Problem+Solver+%26+Code+Enthusiast;Always+Learning+New+Technologies" alt="Typing SVG" />
  </p>

  <!-- Profile Views Counter -->
  <p align="center">
    <img src="https://komarev.com/ghpvc/?username=isamchajia&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />
  </p>
</div>

---

## 🚀 About Me
<img align="right" alt="Coding" width="400" src="https://raw.githubusercontent.com/devSouvik/devSouvik/master/gif3.gif">

- 🔭 Currently working on **innovative web development projects**
- 🌱 Learning **Python** and exploring **automation with Appium**
- 💻 Passionate about **Front-End Development & UI/UX**
- 🛠️ Love building **responsive and interactive web applications**
- 🧩 Enjoy **solving coding puzzles** and **automating tasks**
- 📫 Reach me at: **isamchajia@gmail.com**
- ⚡ Fun fact: **I debug with coffee and solve problems with creativity!** ☕

---

## 🛠️ Tech Stack & Tools
## 🛠️ Tech Stack & Tools
<div align="center">
  ### 💻 Programming Languages
  <p>
    <img src="https://skillicons.dev/icons?i=html,css,js,php,python,mysql,java,c,csharp,ruby,go,swift,kotlin,dart,ts" />
  </p>
  
  ### 🎨 Frameworks & Libraries
  <p>
    <img src="https://skillicons.dev/icons?i=tailwind,bootstrap,react,reactnative,vue,nextjs,nuxt,angular,express,spring,django,flask,laravel" />
  </p>
  
  ### 🔧 Tools & Technologies
  <p>
    <img src="https://skillicons.dev/icons?i=git,github,vscode,figma,docker,kubernetes,jenkins,linux,aws,azure,gcp,supabase" />
  </p>
  
  ### 🗄️ Databases
  <p>
    <img src="https://skillicons.dev/icons?i=mysql,postgresql,mongodb,redis,sqlite,oracle" />
  </p>
  
  ### 🌐 Currently Learning
  <p>
    <img src="https://skillicons.dev/icons?i=react,nodejs,mongodb,graphql,apollo" />
  </p>
</div>


---

## 📊 GitHub Statistics
<div align="center">
  <img width="49%" src="https://github-readme-stats.vercel.app/api?username=isamch&show_icons=true&theme=radical&hide_border=true&count_private=true" />
  <!-- Streak stats removed to avoid 404 error -->
  <img width="70%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=isamch&layout=compact&theme=radical&hide_border=true" />
</div>

---

## 🏆 GitHub Trophies
<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=isamchajia&theme=radical&no-frame=true&no-bg=false&margin-w=4&row=1" />
</div>

---

## 📈 Contribution Graph
<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=isamchajia&theme=react-dark&hide_border=true&area=true" />
</div>

---

## 🎯 Current Focus
<div align="center">
  | 🔥 Current Projects | 🎯 Goals 2024 | 🌟 Interests |
  |:---:|:---:|:---:|
  | Web Development Portfolio | Master React & Node.js | UI/UX Design |
  | Automation Testing Suite | Contribute to Open Source | Mobile Development |
  | Personal Blog Platform | Build 10+ Projects | AI & Machine Learning |
</div>

---

## 🌐 Connect With Me
<div align="center">
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/isamchajia/)
  [![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:isamchajia@gmail.com)
  [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/isamchajia)
</div>

---

## 💡 Random Dev Quote
<div align="center">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical" />
</div>

---

## 🐍 Contribution Snake
<div align="center">
  <img src="https://raw.githubusercontent.com/isamchajia/isamchajia/output/snake.svg" alt="Snake animation" />
</div>

---

<div align="center">
  ### 🎵 Currently Vibing To
  [![Spotify](https://spotify-github-profile.vercel.app/api/spotify-playing)](https://open.spotify.com/user/YOUR_SPOTIFY_USERNAME)
  ---
  **💭 "Code is like humor. When you have to explain it, it's bad." – Cory House**
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer"/>
</div>
\`\`\`

To make your README even more amazing, you'll need to:

1.  **Replace placeholders:**
    *   Change `isamchajia` to your actual GitHub username in all URLs
    *   Update the LinkedIn URL to your actual profile
    *   Add your Spotify username if you want the music widget
2.  **Enable GitHub Actions for Snake Animation:**
    Create `.github/workflows/snake.yml` in your profile repository:

```yaml project="GitHub Profile README" file=".github/workflows/snake.yml" type="code"
name: Generate Snake
on:
  schedule:
    - cron: "0 */6 * * *"
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10

    steps:
      - name: Generate snake.svg
        uses: Platane/snk/svg-only@v2
        with:
          github_user_name: isamchajia
          outputs: dist/snake.svg

      - name: Push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v2.6.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
