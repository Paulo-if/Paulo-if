# ✨Olá!! Eu sou o Paulo Otávio👋

### 😁Mais sobre mim
- 📍Sou do Brasil
- 🌱 Atualmente Estudante de Ciência da Computação na UFJ
- 📚 Estou Constantemente tentnado expandir meu conhecimento.
- ⛏️ Em meu tempo livre gosto de jogar 

## Meios de contato:
[![instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/otaviopaul0/)
[![linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/paulo-ot%C3%A1vio-115a47283/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](https://mail.google.com/mail/u/3/#inbox)

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=Paulo-if&show_icons=true&theme=tokyonight)

## Tecnologias que estou aprendendo:
<div style="display: inline_block"><br/>
<img align="center" alt="c" src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white">
<img align="center" alt="python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
</div>

<div align="center">
  <img height="200" src="https://i.gifer.com/4hsh.gif"  />
</div>

### cobrinha
name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: rafaballerini
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

