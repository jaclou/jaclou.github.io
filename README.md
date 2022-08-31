To get this running from scratch, I did the following:

- I forked [alshedivat/al-folio](https://github.com/alshedivat/al-folio) to `jaclou/jaclou.github.io` (only forked the `master` branch, as is default).
- I cloned the result to my local machine: `gh repo clone jaclou/jaclou.github.io`
- I set my ruby version: `chruby 3.1.1` (so the following command would install gems in a contained place)
- I installed the gems with bundler: `bundle install`
- I previewed the site locally with `bundle exec jekyll serve`
- I edited `_config.yml` to have 
  ```yaml
  url: https://jaclou.github.io
  baseurl: # empty
  ```
- I checked that Github's Settings > Pages had
  - Build and deployment: Source = Deploy from a branch
  - Branch = gh-pages / (root), and clicked Save.
- In the Actions tab, I saw :white_check_mark:__pages build and deployment__

Success.  The site is live.


see readme at [alshedivat/al-folio](https://github.com/alshedivat/al-folio) for rest of info.
