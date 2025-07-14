---
name: 🎮 Rock Paper Scissors
about: Play Rock Paper Scissors with Isam!
title: '🎮 Rock Paper Scissors Game'
labels: game, fun
assignees: isamchajia
---

## 🎮 Let's Play Rock Paper Scissors!

Choose your move by commenting below:

- 🗿 **Rock**
- 📄 **Paper** 
- ✂️ **Scissors**

I'll respond with my move and let you know who wins! 🏆

### Current Score:
- You: 0
- Isam: 0

*Good luck! 🍀*
\`\`\`

**b. `tic-tac-toe.md`**
```yaml project="GitHub Profile Games" file=".github/ISSUE_TEMPLATE/tic-tac-toe.md" type="code"
---
name: ⭕ Tic Tac Toe
about: Play Tic Tac Toe with Isam!
title: '⭕ Tic Tac Toe Game'
labels: game, fun
assignees: isamchajia
---

## ⭕ Let's Play Tic Tac Toe!

\`\`\`
 1 | 2 | 3 
-----------
 4 | 5 | 6 
-----------
 7 | 8 | 9 
\`\`\`

You are **X**, I am **O**. 

Comment with the number (1-9) where you want to place your X!

*Let the games begin! 🎮*
\`\`\`

**c. `daily-coding-riddle.md`**
```yaml project="GitHub Profile Games" file=".github/ISSUE_TEMPLATE/daily-coding-riddle.md" type="code"
---
name: 🧩 Daily Coding Riddle
about: Challenge your brain with a coding riddle!
title: '🧩 Daily Coding Riddle'
labels: riddle, fun
assignees: isamchajia
---

## 🧩 Daily Coding Riddle Challenge!

Here's today's riddle:

**What has keys but no locks, space but no room, and you can enter but can't go inside?**

Comment your answer below! I'll reveal the solution in a few days.

*Hint: Think about everyday objects!*
\`\`\`

**d. `random-tech-tip.md`**
```yaml project="GitHub Profile Games" file=".github/ISSUE_TEMPLATE/random-tech-tip.md" type="code"
---
name: 🎲 Random Tech Tip
about: Get a random tech tip from Isam!
title: '🎲 Random Tech Tip'
labels: tip, tech
assignees: isamchajia
---

## 🎲 Your Random Tech Tip!

Here's your random tech tip:

**Tip:** Always use meaningful variable names. Your future self will thank you!

*Click to get another tip!*
\`\`\`

**e. `collaboration-opportunity.md`**
```yaml project="GitHub Profile Games" file=".github/ISSUE_TEMPLATE/collaboration-opportunity.md" type="code"
---
name: 🤝 Collaboration Opportunity
about: Let's work together on something amazing!
title: '🤝 Collaboration Opportunity'
labels: collaboration, project
assignees: isamchajia
---

## 🤝 Let's Collaborate!

Hi Isam!

I'd love to collaborate on:
- [ ] Web Development Project
- [ ] Open Source Contribution
- [ ] Learning Together
- [ ] Other (please specify)

Details:
[Please describe your idea or what you'd like to work on]

My GitHub profile: [Your GitHub Profile Link]
My contact email: [Your Email]

Looking forward to hearing from you!
\`\`\`

### 2. Enable GitHub Actions for Snake Animation

This will generate the `github-contribution-grid-snake-dark.svg` file dynamically. Create a file named `.github/workflows/snake.yml` in your profile repository:

```yaml project="GitHub Profile README - Snake Action" file=".github/workflows/snake.yml" type="code"
name: Generate Snake

on:
  schedule:
    - cron: "0 */6 * * *" # Runs every 6 hours
  workflow_dispatch: # Allows manual triggering

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    
    steps:
      - name: Generate snake.svg
        uses: Platane/snk/svg-only@v2
        with:
          github_user_name: isamchajia # Replace with your GitHub username
          outputs: dist/github-contribution-grid-snake-dark.svg # Output path
          
      - name: Push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v2.6.0
        with:
          target_branch: output # This branch will store the generated SVG
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # GitHub token for pushing
