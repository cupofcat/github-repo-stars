# github-repo-stars
## Usage
http://cupofcat.github.io/repo-stars/index.html?kubernetes/autoscaler

## Setup as subdirectory in a GitHub Page repo
```shell
git remote add upstream git@github.com:cupofcat/github-repo-stars.git
git config remote.upstream.pushurl "DO NOT PUSH TO UPSTREAM FROM HERE"
git fetch upstream
git subtree add --prefix repo-stars upstream master --squash
git subtree pull --prefix repo-stars upstream master --squash
git push
```

To update you can just use:
```shell
git fetch upstream && git subtree pull --prefix repo-stars upstream master --squash
```

Read more on git subtree here: https://www.atlassian.com/blog/git/alternatives-to-git-submodule-git-subtree