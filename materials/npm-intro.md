# NPM (Node Package Manager)

## What is NPM?

**NPM** (Node Package Manager) is the default package manager for Node.js. It
serves two primary functions:

1. **Online Repository**: NPM hosts a vast repository of open-source packages
   and modules for Node.js, which you can search and explore at
   [search.npmjs.com](https://search.npmjs.com/).
2. **Command Line Utility**: NPM provides a command-line tool for managing
   packages, handling version control, and managing dependencies for Node.js
   projects.

![NPM Logo](https://upload.wikimedia.org/wikipedia/commons/e/ec/Npm-logo.svg)

## Core Features

- **Package Management**: Download and install packages from the NPM registry.
- **Version Control**: Manage package versions and update dependencies.
- **Script Management**: Run custom scripts defined in your `package.json` file.
- **Dependency Management**: Automatically handle dependencies for your
  projects.

## Basic NPM Commands

### 1. Check NPM Version

To check the installed version of NPM, use the following command:

```sh
npm --version
```

### 2. Initialize a New Project

To create a `package.json` file for a new Node.js project, run:

```sh
npm init
```

You will be prompted to enter details like the project name, version, and
description. For a quicker setup with default values, use:

```sh
npm init -y
```

### 3. Install Packages

To install a package and add it to the `dependencies` section of `package.json`,
use:

```sh
npm install <package-name>
```

To install a package as a development dependency, use:

```sh
npm install <package-name> --save-dev
```

### 4. Update Packages

To update a specific package to the latest version:

```sh
npm update <package-name>
```

To update all packages listed in `package.json`:

```sh
npm update
```

### 5. Install All Dependencies

To install all the dependencies listed in `package.json`, use:

```sh
npm install
```

### 6. Run Scripts

To run a script defined in the `scripts` section of `package.json`, use:

```sh
npm run <script-name>
```

For example, to start a development server with a script called `start`, you
would run:

```sh
npm run start
```

### 7. Uninstall Packages

To remove a package and also remove it from `package.json`, use:

```sh
npm uninstall <package-name>
```

To uninstall a package but keep it in `package.json`, use:

```sh
npm uninstall <package-name> --no-save
```

### 8. View Package Information

To get detailed information about a package, including its dependencies,
version, and more:

```sh
npm info <package-name>
```

### 9. Search for Packages

To search for packages in the NPM registry:

```sh
npm search <query>
```

### 10. Audit Dependencies

To check for vulnerabilities in your dependencies:

```sh
npm audit
```

To fix vulnerabilities:

```sh
npm audit fix
```

## Advanced NPM Features

### 1. Workspaces

NPM Workspaces allow you to manage multiple packages within a single repository.

- **Define Workspaces** in `package.json`:

  ```json
  {
    "workspaces": ["packages/*"]
  }
  ```

- **Run Commands Across All Workspaces**:

  ```sh
  npm run <script> --workspace <workspace-name>
  ```

### 2. NPM Scripts

Scripts in `package.json` allow you to automate common tasks.

- **Example `scripts` Section**:

  ```json
  "scripts": {
    "start": "node app.js",
    "test": "mocha test/",
    "build": "webpack"
  }
  ```

- **Run `start` Script**:

  ```sh
  npm start
  ```

### 3. Creating and Publishing Packages

- **Create a Package**:

  - Create a directory and add a `package.json` file.
  - Add your code and documentation.
  - Use the following command to publish:

    ```sh
    npm publish
    ```

- **Scope Packages**:

  - Use scoped packages to publish under a specific namespace, e.g.,
    `@username/package-name`.

    ```sh
    npm publish --access public
    ```

### 4. Global vs Local Packages

- **Install Package Globally**:

  ```sh
  npm install -g <package-name>
  ```

  This makes the package available anywhere on your system.

- **Install Package Locally**:

  ```sh
  npm install <package-name>
  ```

  This installs the package in the `node_modules` directory of your project.

### 5. Configuring NPM

To view or modify your NPM configuration settings:

- **View Configuration**:

  ```sh
  npm config list
  ```

- **Set a Configuration Value**:

  ```sh
  npm config set <key> <value>
  ```

- **View Global Configuration File**:

  ```sh
  npm config edit
  ```

## Common Issues and Solutions

- **Issue: `npm install` Fails**

  **Solution**: Check for missing or incorrect permissions, update NPM, or clear
  the cache:

  ```sh
  npm cache clean --force
  ```

- **Issue: Dependency Conflicts**

  **Solution**: Resolve version conflicts by reviewing the `package.json` or
  using `npm outdated` to check for updates.

  ```sh
  npm outdated
  ```

## Resources

- [Official NPM Documentation](https://docs.npmjs.com/)
