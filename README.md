
Instructions for setting up username.github.com *
  Create a repo named username.github.com
  Push a `master` branch to GitHub and enjoy!
Instructions for setting up username.github.com/repo-name *
Caution: make your working directory clean before you do this (either stash or commit), otherwise this will lose any changes you've made to your project since the last commit.
  cd /path/to/repo-name
  git symbolic-ref HEAD refs/heads/gh-pages
  rm .git/index
  git clean -fdx
  echo "My GitHub Page" > index.html
  git add .
  git commit -a -m "First pages commit"
  git push origin gh-pages
