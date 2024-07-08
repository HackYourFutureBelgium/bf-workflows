# Git and GitHub

## Why Use Git and GitHub?

Git and GitHub are essential tools in modern software development, facilitating
efficient version control and collaboration among developers. They enable you
to:

- Track changes to your code over time.
- Collaborate seamlessly with other developers.
- Maintain multiple versions of your project.
- Host and share your code publicly or privately.

## Git vs. GitHub: Understanding the Difference

- **Git**: A distributed version control system that helps you manage and keep
  track of changes in your codebase. It is a command-line tool that allows you
  to record the history of your project.
- **GitHub**: A cloud-based platform that hosts Git repositories. It provides a
  web-based interface to manage your repositories, collaborate with others, and
  utilize additional features such as issue tracking, project management, and
  GitHub Pages for hosting websites.

## Connecting Git to Your GitHub Account

Before you can interact with GitHub from your local machine, you need to
configure Git with your GitHub credentials.

### Setting Your Git Username

```sh
git config --global user.name "Your GitHub Username"
```

### Setting Your Git Email

```sh
git config --global user.email "your.email@example.com"
```

## Starting a New Project on GitHub

### Step 1: Create a Repository on GitHub

1. Log in to your GitHub account.
2. Click on the `+` icon in the upper right corner and select "New repository".
3. Fill in the repository name, description (optional), and choose the
   repository visibility (public or private).
4. Click "Create repository".

### Step 2: Add Collaborators

1. Navigate to the repository on GitHub.
2. Click on "Settings" > "Collaborators & teams".
3. Add collaborators by entering their GitHub usernames.

### Step 3: Enable GitHub Pages (Optional)

1. Go to the repository settings.
2. Scroll down to the "GitHub Pages" section.
3. Choose a source branch for GitHub Pages and click "Save".

### Step 4: Protect Your Main Branch (Optional)

1. In the repository settings, go to "Branches".
2. Under "Branch protection rules", add a rule for the `main` branch.
3. Configure the desired protections, such as requiring pull request reviews.

### Step 5: Clone the Repository Locally

To work on your project locally, you need a local copy of the repository.

```sh
git clone https://github.com/username/repository.git
```

## Pushing and Pulling Code

### Pushing Changes to the Main Branch

After making changes and committing them locally, push the updates to the remote
`main` branch.

```sh
git push origin main
```

### Pushing Changes to Another Branch

If you're working on a different branch, push your changes to the corresponding
remote branch.

```sh
git push --set-upstream origin branch-name
```

### Pulling Updates from the Remote Repository

To fetch and integrate changes from the remote repository to your local `main`
branch:

```sh
git pull origin main
```

To fetch and integrate changes to another branch:

```sh
git pull origin branch-name
```

## Basic Git Commands

### Adding Changes

Stage changes for the next commit.

```sh
git add .
```

### Committing Changes

Record the staged changes in the repository.

```sh
git commit -m "Your commit message"
```

### Viewing Commit History

Display the history of commits in the repository.

```sh
git log
```

### Creating a New Branch

Create and switch to a new branch.

```sh
git checkout -b new-branch-name
```

### Merging Branches

Merge the specified branch into the current branch.

```sh
git merge branch-name
```
