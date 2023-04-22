# Git

> What is git?

## Git(Version control system)

is the most popular version control system.

![git over time](../assets//change-files.png)

- `Git` is software that runs locally. Your files and their history are stored
  on your computer.
- `Git` tracks the changes you make to files.
- `Git` also makes collaboration easier, allowing changes by multiple people to
  all be merged into one source.

![git](../assets/git.png)

### Git Repositories\*\*

It is a hidden subfolder contains all of the project files and the entire
revision history.

### The Three States

Git has three main states that your files can reside in: modified, staged, and
committed:

- _Modified_: means that you have changed the file(s) but have not committed it
  yet.
- _Staged_: means that you have added the changed file(s) to the `staging area`
- _committed_: means the changed file(s) has been committed.

![git states](../assets/git-states.png)

### Git Branching

_Git_ allows you to create different branches, where you can add your code
without affecting the `master/main` branch. Also developers can work on
different branch at the same time.

![git branches](../assets//branches.png)

### Git Merging

_Git merge_ it is combining two separate development histories into one. In
other words, you can merge code from a separate branch into the main branch to
integrate the changes.

### git most used commands

Add `user name` to git

```Markdown
  git config --global user.name "your gitHub user name"
```

Add `email` to git

```Markdown
  git config --global user.email "your email"
```

Make `VS code` the default editor

```Markdown
git config --global core.editor "code --wait"
```

Handle the end line <br> Mac or Linux

```Markdown
git config --global core.autocrlf input
```

Windows

```Markdown
git config --global core.autocrlf true
```

See all git global configuration in your `VS code`

```Markdown
git config --global -e
```

Initialize empty git repo

```Markdown
git init
```

List all the untracked files

```Markdown
git status
```

Add file(s) to staging area

```Markdown
git add <file name>
```

Add all file(s) to staging area

```Markdown
git add .
```

Remove file(s) from staging area

```Markdown
git reset <file name>
```

Commit changes

```Markdown
git commit -m " descriptive message"
```

Save changes without committing them temperately

```Markdown
git stash
```

To restore or reapply the stashed changes

```Markdown
git stash apply
```

To create a new branch

```Markdown
git branch <branch name>
```

To switch to the new branch

```Markdown
git checkout <branch name>
```

To create a new branch and switch to it

```Markdown
git checkout -b <branch name>
```

To revert a commit

```Markdown
git revert <A commit hash>
```

To reset the changes

```Markdown
git reset
```

To display the most recent commits

```Markdown
git log
```

To compare changes

```Markdown
git diff
```

To integrate changes from one branch onto another

```Markdown
git rebase <branch name>
```
