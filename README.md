[![GitHub Actions](https://img.shields.io/github/actions/workflow/status/heinrichreimer/reimersoftware-portfolio/ci.yml?branch=master&style=flat-square)](https://github.com/heinrichreimer/reimersoftware-portfolio/actions/workflows/ci.yml)

# 🌐 portfolio

Reimer Software's (former) [portfolio website](https://reimer.software).

## Build

We have bash scripts in place to simplify deployments:
- [`build.sh`](build.sh) which builds the static sites
  using [Jekyll](https://jekyllrb.com/) and checks the HTML output
  using [html-proofer](https://github.com/gjtorikian/html-proofer).
- [`refresh-portfolio.sh`](https://gist.github.com/heinrichreimer/0bee5be4af58d316e5fda61b82fd3d29)
  which runs on my web server, pulls the GitHub repo, launches
  the build script and then - if everything worked as expected -
  deploys the updated site to my servers Apache directory.

Updating the portfolio is as simple as typing `./refresh-portfolio.sh` into SSH - which is done by GitHub Actions :+1:
