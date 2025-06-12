# WIESP static site

Theme: [minimal-mistakes](https://mmistakes.github.io/minimal-mistakes/)

## Run locally

- Install [Jekyll](https://jekyllrb.com/docs/installation/)
- Follow [GitHub instructions](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)
- Edit `_config.yml`: 
  - Comment out the `remote-theme` 
  - Uncomment out the `theme`
- Run:

```bash
bundle install
bundle exec jekyll serve
```
- On final commit to Github, make sure to change the `_config.yml` back again, so the `remote-theme` is active.