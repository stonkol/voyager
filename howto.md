## How to commit in the Middle Ages

1. Make some changes or create a file to commit (e.g., `echo "Hello" > file.txt` and `git add file.txt`).
2. Before committing, set the environment variables in your terminal for the desired commit date (e.g., January 1, 1970):

```sh
export GIT_AUTHOR_DATE="1970-01-01 12:00:00"
export GIT_COMMITTER_DATE="1970-01-01 12:00:00"
```
3. Then commit and push:

```sh
git commit -m "Commit from 1970"
git push origin main
```

## Important notes:

- The environment variables affect only the current shell session or script. If you make another commit without resetting or unsetting them, the same date will be used again.
- You can also set the commit date directly using:

```sh
GIT_COMMITTER_DATE="1970-01-01 12:00:00" git commit --date="1970-01-01 12:00:00" -m "Commit from 1970"
```
