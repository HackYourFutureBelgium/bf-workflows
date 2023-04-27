# Group Introduction

> use this starter repository:
> [Markdown template repository](https://github.com/HackYourFutureBelgium/template-markdown)

Find a time to meet with your study group and build a get-to-know-you repository
with one markdown file per person in your group. This doesn't need to be
anything fancy. Your focus should be on getting to know each other and learning
to work on a shared repository.

When you're ready to start your group repo, create a new issue in the class repo
using the `deliverable` template and add the following labels `group`,
`deliverable` and `week-1` labels. Fill out the project's description, list your
group members, and paste this checklist into your issue before
[adding it to the Class Projects board](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/adding-issues-and-pull-requests-to-a-project-board):

> PS. check out other HYF classes for inspiration

## Checklists

- For your group's `deliverable` issue in the class repo:

  ```markdown
  <!-- replace the _ with the correct user name and repo -->

  - [ ] [repo](https://github.com/_/_)
  - [ ] [many small, well-named commits](https://github.com/_/_/commits)
  - [ ] a nice README
  - [ ] one well-named file per person
  - [ ] [one pull requests for each group member](https://github.com/_/_/pulls)
    - [ ] linting checks pass
    - [ ] code review checklist is complete
    - [ ] the reviewer merged the code
  ```

- For your individual PRs in your group repository

  ```markdown
  - Setup: GitHub
    - [ ] created this issue
    - [ ] assigned myself
    - [ ] moved the issue to the project board
  - Setup: local
    - [ ] pulled the most recent code from `main`/`master`
    - [ ] created a new branch for my introduction
  - Writing the content:
    - [ ] added my intro file in `/people` according to group conventions
    - [ ] linked to my file from `/README.md` according to group conventions
  - Before pushing my branch:
    - [ ] formatted the code
    - [ ] fixed all spelling mistakes and added new words to the dictionary
    - [ ] fixed all linting mistakes
  - After pushing my branch:
    - [ ] created a new PR linked to this issue
    - [ ] make sure all of the checks passed
    - [ ] assigned someone to review and merge my PR
  ```

## Steps

0. create a new issue on your class `home` repo, ex:
   `group1 : workflows : intro` , labels : `group`,`deliverable` and `week-1`
   and add the first checklist to your issue.
1. one of you will be the `project leader`
2. create a new repo on your `class organization` using the template  
   [Markdown template repository](https://github.com/HackYourFutureBelgium/template-markdown)
3. go to setting, turn on gitHub pages, add collaborators and give them `write`
   access, protect `master/main` branch and turn on discussions
4. discus with your teammates about the project, how many branches you will need
   to create? how many files?
5. create a `project board`
6. create your issues, `one issue for each file` and add them to the
   `project board`
7. create a branch add your file ex: `samir.md` add your info.
8. run all code quality check.
9. run `git pull origin main`
10. if you have a conflict resolved it.
11. add your changes and commit them.
12. push your changes and make a `PR`
13. add the checklist to your `PR` and add `reviewers` and link the `issue`
