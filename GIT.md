# Git utils

Creating a repository on mac OS.

There is an automatically created file that tracks every single state of the folder on MacOS which is called `.DS_Store` this can be removed from git traking with the following command.

```bash
find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch
```

Creating the `.gitignore` file for repositories on MacOS

```bash
echo .DS_Store >> .gitignore
```

Adding the `.gitignore` file to the repository

```bash
git add .gitignore
git commit -m '.DS_Store banished!'
```