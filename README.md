# www.surfstationfoundation.org

## initial setup

- create a new public repository named `www.surfstationfoundation.org`
- go to https://github.com/surfstationfoundation/www.surfstationfoundation.org/settings and configure the new repo
- `mkdir www.surfstationfoundation.org`
- `cd www.surfstationfoundation.org`
- `git init`
- `git config user.name surfstationfoundation`
- `git config user.email 'surfstationfoundation@users.noreply.github.com'`
- `git config pull.ff only`
- `git add -A`
- `git commit -m 'first commit'`
- `git branch -M main`
- `git remote add origin https://github.com/surfstationfoundation/www.surfstationfoundation.org.git`
- `git switch --orphan gh-pages`
- `git commit --allow-empty --allow-empty-message`
- `git push -u origin gh-pages`
- `git switch main`
- `git push -u origin main`
- go to https://github.com/surfstationfoundation/www.surfstationfoundation.org/settings/branches and set main as the default branch

## dev notes

bundle install;

cd www;

JEKYLL_ENV=development bundle exec jekyll serve --host 0.0.0.0;

or

JEKYLL_ENV=production bundle exec jekyll build;

for example:

cd /path-to/www.surfstationfoundation.org/www/ && git pull && bundle install && JEKYLL_ENV=production bundle exec jekyll build
