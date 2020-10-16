# google-python-style-precommit-hook
A pre-commit hook to format python code files.

The pre-commit.sh file are totally copied from [google yapf project](https://github.com/google/yapf/tree/master/plugins#git-pre-commit-hook).

# Usage
You can use it with [pre-commit](https://pre-commit.com/) or in a naive [Git hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) way.

## Pre-commit way (Recommend) 
Add the follow lines to your .pre-commit-config.yaml
```
-   repo: https://github.com/chengzhang/google-python-style-precommit-hook.git
    hooks:
    -   id: google-python-style
```

## Git hooks way
Ref to [google yapf](https://github.com/google/yapf/tree/master/plugins#git-pre-commit-hook)
