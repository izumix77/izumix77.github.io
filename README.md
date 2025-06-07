# izumix77.github.io

This is a personal blog and content site built with [Clean Blog Jekyll](https://startbootstrap.com/themes/clean-blog-jekyll/), customized and deployed via GitHub Actions and GitHub Pages.

## 📦 Project Overview

- **Framework**: Jekyll (Theme: Clean Blog Jekyll)
- **Hosting**: GitHub Pages (deployment from `master` branch)
- **CI/CD**: GitHub Actions (`.github/workflows/jekyll.yml`)

## 🚀 Deployment Workflow

This site is automatically built and deployed every time a commit is pushed to the `master` branch.

Main steps:

```yaml
- uses: actions/checkout@v4
- uses: ruby/setup-ruby@v1
- uses: actions/upload-pages-artifact@v2
- uses: actions/deploy-pages@v3
✅ Ruby version: 3.2+
✅ Gemfile.lock includes platform x86_64-linux for compatibility with GitHub Actions

🌐 Live Site
You can view the site here:
👉 https://izumix77.github.io

🛠 Local Development
To run the site locally:

bundle install
bundle exec jekyll serve
Then open your browser to:
http://localhost:4000

🗒 Notes
Customized from the official Start Bootstrap Jekyll Theme

Ruby and bundler setup required for local development

Uses GitHub Actions for fully automated deployment to GitHub Pages

Feel free to fork or use this setup as a boilerplate for your own static site projects.