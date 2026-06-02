  GNU nano 9.0     5_snake-1.yml
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: Prem2868
          outputs: |\
            dist/github-contribution-grid-snake>
            dist/github-contribution-grid-snake>
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKE>
      - uses: crazy-max/ghaction-github-pages@v>
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKE>


