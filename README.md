## Olá! Eu sou Vanessa Avila 🖐️
- 🤔 Estundante de Analise de Teste de Software 
- 😄 Pronouns: ela/dela

 
 
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/_sousa97_)
 
![Vanessa Avila GitHub stats](https://github-readme-stats.vercel.app/api?username=ProjetoAuroraBoreal&show_icons=true&theme=dracula&count_private=true)

## Tecnologias que eu uso no meu dia

<div style="display: inline_block">
  <img align="center" alt="html5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img align="center" alt="css" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img align="center" alt="js" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />


<a href="https://github.com/ProjetoAuroraBoreal/github-readme-stats">
  <img height=200 align="center" src="https://github-readme-stats.vercel.app/api?username=ProjetoAuroraBoreal" />
</a>
<a href="https://github.com/ProjetoAuroraBoreal/convoychat">
  <img height=200 align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=ProjetoAuroraBoreal&layout=compact&langs_count=8&card_width=320" />
</a>
 @@ -55,9 +55,9 @@ Available as github action. It can automatically generate a new image each day.
      dist/github-snake-dark.svg?palette=github-dark
      dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
    env:
      # a github token is required to fetch the contribution calendar from github API
      GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  env:
    # a github token is required to fetch the contribution calendar from github API
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

[example with cron job](https://github.com/Platane/Platane/blob/master/.github/workflows/main.yml#L25-L33)







name: generate animation

on:
  # run automatically every 24 hours
  schedule:
    - cron: "0 */24 * * *" 
  
  # allows to manually run the job at any time
  workflow_dispatch:
  
  # run on every push on the master branch
  push:
    branches:
    - master
    
  

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    
    steps:
      # generates a snake game from a github user (<github_user_name>) contributions graph, output a svg animation at <svg_out_path>
      - name: generate github-contribution-grid-snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          
          
      # push the content of <build_dir> to a branch
      # the content will be available at https://raw.githubusercontent.com/<github_user>/<repository>/<target_branch>/<file> , or as github page
      - name: push github-contribution-grid-snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

</div>







<br/>


<!--
**ProjetoAuroraBoreal/ProjetoAuroraBoreal** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

  <img align="center" alt="ts" src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" />
  <img align="center" alt="react" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img align="center" alt="nodejs" src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" />
-->


