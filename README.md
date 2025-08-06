name: Generate Snake Animation

on:
  schedule:
    - cron: "0 */6 * * *"
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    permissions: 
      contents: write
      
    steps:
      - name: Generate snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          
          # FINAL FIX: Reverts to the dark theme but makes the background plane transparent
          outputs: |
            dist/snake-dark.svg?palette=github-dark&color_bg=#00000000

      - name: Push to GitHub
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
