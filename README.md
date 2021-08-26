# git-rubocop

```
Runs the rubocop command on the files included in git diff.

Usage: git rubocop [git-diff-args...] -- [rubocop-args...]

To install, add this script to your PATH, then run one of the following:

    git config --global alias.rubocop '!git-rubocop' # All repos
    git config alias.rubocop '!git-rubocop'          # Current repo only

Examples:
 • Run on unstaged files:                git rubocop
 • Run on staged files:                  git rubocop --staged
 • Run on all changed files:             git rubocop head
 • Autocorrect all changed files:        git rubocop head -- -A
 • Run on files changed between commits: git rubocop head~2 head~1
 • Run on files differing from master:   git rubocop origin/master

Options:
    -h       Print this message (Don't use --help)
```
