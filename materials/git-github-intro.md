# Git and GitHub

> Why do I need to use Git and GitHub?

Git and GitHub are common tools used in programming. They help you manage
different versions of your code and collaborate with other developers.

> What is the difference between Git and GitHub?

`Git` is a version control system that manages and keeps track of your code.
`GitHub`, on the other hand, is a service that let you host, share, and manage
your code files on the internet.

> How can I connect my GitHub account to git?

To set your git user name

```Markdown
git config --global user.name "your gitHub's user name"
```

To set your git email

```Markdown
git config --global user.email "your gitHub's email"
```

> How can I start working on a project?

1- You need to create a repository on `GitHub`. Note: choose the right `owner`.

2- You can add collaborators.

3- you can turn on github pages.

4- you can protect your `main` branch.

5- you need to have your own local copy, so you will be able to add your code.

```Markdown
git clone <repo URL>
```

To push your code to a remote repo (GitHub) `main` after adding and committing
your changes

```Markdown
git push
```

To push your code to a remote repo (GitHub) `another-branch` after adding and
committing your changes

```Markdown
git push --set-upstream origin <branch name>
```

To pull the latest update from a remote repo (GitHub), to the `main` branch

```Markdown
git pull
```

To pull the latest update from a remote repo (GitHub), to `another-branch`
branch

```Markdown
git pull origin main
```
