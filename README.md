<h1 align="center">Hi there, I'm Limon! 🚀</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=F75C7E&width=435&lines=Web+Developer+%7C+Freelancer;Tech+Enthusiast+%7C+Dream+Chaser;Building+the+Future+One+Line+of+Code+at+a+Time!" />
</p>

### 🌟 About Me  
- 🔭 I’m currently working on web development projects.  
- 🌱 Learning and improving every day!  
- 💡 Exploring freelancing and business opportunities.  

### ⚡ GitHub Stats  
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=your-username&show_icons=true&theme=radical" width="400"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=your-username&theme=radical" width="400"/>
</p>

### 💻 Languages & Tools  
<p align="center">
  <img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,git,github,vscode" />
</p>name: Update README with a Quote

on:
  schedule:
    - cron: "0 * * * *" # Runs every hour

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repo
        uses: actions/checkout@v3

      - name: Fetch Quote
        run: curl -s https://api.quotable.io/random | jq -r '.content' > quote.txt

      - name: Update README
        run: |
          sed -i "s|<!--QUOTE-->|$(cat quote.txt)|" README.md
          git config --global user.name "github-actions[bot]"
          git config --global user.email "github-actions[bot]@users.noreply.github.com"
          git commit -am "Updated quote"
          git push![Visitor Count](https://komarev.com/ghpvc/?username=your-username&color=blue)> <!--QUOTE-->THE MAGIC YOU ARE LOKING FOR IS IN THE WORK YOU ARE AVOIDING
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=F75C7E&center=true&width=600&lines=THE+MAGIC+YOU+ARE+LOOKING+FOR;IS+IN+THE+WORK+YOU+ARE+AVOIDING" />
</p>
