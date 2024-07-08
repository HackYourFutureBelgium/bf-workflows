# Visual Studio Code (VS Code)

## What is Visual Studio Code?

**Visual Studio Code** (VS Code) is a powerful, open-source code editor
developed by Microsoft. It is designed to be lightweight, yet feature-rich,
making it an ideal tool for building and debugging modern web and cloud
applications. VS Code supports a wide range of programming languages and offers
a variety of tools and extensions to enhance your development workflow.

![Visual Studio Code](https://code.visualstudio.com/assets/docs/getstarted/keybindings/vscode-intro.png)

For more information, visit the
[official VS Code website](https://flaviocopes.com/vscode/).

## Key Features

### 1. **Cross-Platform**

VS Code is available for Windows, macOS, and Linux, ensuring a consistent
development experience across different operating systems.

### 2. **Integrated Git Control**

VS Code comes with built-in Git support, allowing you to manage your version
control directly from the editor.

- **Git Commands**:
  - **Stage Changes**: `Ctrl+Shift+G` (Windows/Linux) or `Cmd+Shift+G` (macOS)
  - **Commit Changes**: Enter commit message and click the checkmark icon.
  - **Push Changes**: `Ctrl+Shift+P` and type `Git: Push`

### 3. **Debugging Support**

VS Code offers a robust debugging environment with support for breakpoints,
watch expressions, and more.

- **Start Debugging**:

  - **Run**: `F5`
  - **Debug Console**: `Ctrl+Shift+Y` (Windows/Linux) or `Cmd+Shift+Y` (macOS)

- **Configure Debugging**:
  - Create a `launch.json` file to set up your debugging configuration.

### 4. **Extensions Marketplace**

VS Code has a rich ecosystem of extensions available through the
[Extensions Marketplace](https://marketplace.visualstudio.com/vscode).

- **Popular Extensions**:

  - **Prettier**: Code formatter
  - **ESLint**: Linting for JavaScript and TypeScript
  - **Live Server**: Launch a local development server
  - **Debugger for Chrome**: Debug your JavaScript code in the Chrome browser

- **Install Extensions**:

  ```sh
  Ctrl+Shift+X
  ```

### 5. **Integrated Terminal**

VS Code features an integrated terminal for running shell commands.

- **Open Terminal**:
  - **Windows/Linux**: `` Ctrl+` ``
  - **macOS**: `` Cmd+` ``

### 6. **Code Editing Features**

VS Code offers various features to enhance your coding experience:

- **Syntax Highlighting**: Supports a wide range of programming languages.
- **Code Snippets**: Predefined templates for common code structures.
- **IntelliSense**: Code completion suggestions and parameter info.

### 7. **Code Navigation**

VS Code provides tools for easy navigation within your codebase.

- **Go to Definition**: `F12`
- **Find References**: `Shift+F12`
- **Peek Definition**: `Alt+F12`

### 8. **Code Refactoring**

Refactor your code with built-in tools.

- **Rename Symbol**: `F2`
- **Extract Method**: `Ctrl+Shift+R` (Windows/Linux) or `Cmd+Shift+R` (macOS)

### 9. **Themes and Customization**

VS Code allows you to customize the editor’s appearance.

- **Change Theme**:

  - **Command Palette**: `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (macOS)
    and type `Color Theme`.

- **Popular Themes**:
  - **One Dark Pro**
  - **Material Theme**
  - **Dracula Official**

### 10. **Workspace Management**

Manage different projects and their configurations with workspaces.

- **Open a Workspace**:

  - **Command Palette**: `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (macOS)
    and type `Open Workspace`.

- **Save Workspace**:
  - **File Menu**: `File > Save Workspace As...`

## Basic Commands

Here are some common commands and their shortcuts:

| Command              | Windows/Linux  | macOS         |
| -------------------- | -------------- | ------------- |
| Open Command Palette | `Ctrl+Shift+P` | `Cmd+Shift+P` |
| Open File            | `Ctrl+O`       | `Cmd+O`       |
| Save File            | `Ctrl+S`       | `Cmd+S`       |
| Close File           | `Ctrl+W`       | `Cmd+W`       |
| Split Editor         | `Ctrl+\`       | `Cmd+\`       |
| Search               | `Ctrl+Shift+F` | `Cmd+Shift+F` |
| Find                 | `Ctrl+F`       | `Cmd+F`       |
| Replace              | `Ctrl+H`       | `Cmd+H`       |
| Show Explorer        | `Ctrl+Shift+E` | `Cmd+Shift+E` |
| Show Extensions      | `Ctrl+Shift+X` | `Cmd+Shift+X` |
| Open Settings        | `Ctrl+,`       | `Cmd+,`       |

## Advanced Features

### 1. **Remote Development**

VS Code supports remote development through extensions like:

- **Remote - SSH**: Connect to remote machines.
- **Remote - Containers**: Work inside a Docker container.
- **Remote - WSL**: Develop in the Windows Subsystem for Linux.

### 2. **Settings and Configurations**

Customize VS Code settings through the `settings.json` file.

- **Open Settings**:
  - **File Menu**: `File > Preferences > Settings`
  - **Command Palette**: `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (macOS)
    and type `Preferences: Open Settings (JSON)`

### 3. **User and Workspace Settings**

- **User Settings**: Apply settings globally.
- **Workspace Settings**: Apply settings specific to a workspace.

### 4. **Debugging Configuration**

Create or modify the `launch.json` file for advanced debugging configurations.

- **Example `launch.json`**:

  ```json
  {
    "version": "0.2.0",
    "configurations": [
      {
        "type": "node",
        "request": "launch",
        "name": "Launch Program",
        "program": "${workspaceFolder}/app.js"
      }
    ]
  }
  ```

## Extensions

Here are some recommended extensions for different tasks:

| Extension                  | Description                                  |
| -------------------------- | -------------------------------------------- |
| **Prettier**               | Code formatter for various languages.        |
| **ESLint**                 | Linting for JavaScript and TypeScript.       |
| **Live Server**            | Launch a local development server.           |
| **Debugger for Chrome**    | Debug JavaScript code in the Chrome browser. |
| **Bracket Pair Colorizer** | Colorize matching brackets.                  |
| **GitLens**                | Enhance Git capabilities in VS Code.         |

## Resources

- [Official VS Code Documentation](https://code.visualstudio.com/docs)
- [VS Code Marketplace](https://marketplace.visualstudio.com/vscode)
- [VS Code GitHub Repository](https://github.com/microsoft/vscode)
- [VS Code Tips and Tricks](https://code.visualstudio.com/docs/getstarted/tips-and-tricks)
