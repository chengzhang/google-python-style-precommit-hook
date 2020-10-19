# google-python-style-precommit-hook
A pre-commit hook to format python code files. The pre-commit.sh file was totally copied from [google yapf project](https://github.com/google/yapf/tree/master/plugins#git-pre-commit-hook).

# Usage
You can use it with [pre-commit](https://pre-commit.com/) or in a naive [Git hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) way.

## Pre-commit way 
1. create a file named .pre-commit-config.yaml under the root of your git project.
2. Add the follow lines to your .pre-commit-config.yaml
```
repos: 
-   repo: https://github.com/chengzhang/google-python-style-precommit-hook.git
    rev: 0f10b46c22c8c389ce6bc16d71a18c03c74d160c
    hooks:
    -   id: google-python-style
```
3. run
```
pre-commit install
```

## Git hooks way
```
# From the root of your git project.
curl -o pre-commit.sh https://raw.githubusercontent.com/chengzhang/google-python-style-precommit-hook/main/pre-commit.sh
chmod a+x pre-commit.sh
mv pre-commit.sh .git/hooks/pre-commit
```
