# C++ Development Environment - GitHub Codespaces

This repository is configured to provide a ready-to-use C++ development environment within **GitHub Codespaces**. The development environment is defined in the `devcontainer.json` file and includes settings, tools, and extensions that streamline C++ development, including features for static analysis, debugging, and formatting.

## Devcontainer Settings Overview

### 1. **Base Image**
- **Image**: `mcr.microsoft.com/devcontainers/base:ubuntu`
  - The development environment is built on top of an Ubuntu base image, providing a stable and familiar environment for C++ development.
  
### 2. **Installed Features**
The following common utilities and tools are installed in the container:
- **Common Utils**: Basic utilities for working in the terminal.
- **Git**: Version control with Git, ensuring seamless source control management.

### 3. **VS Code Customizations**

- **Minimap Disabled**: 
  - `"editor.minimap.enabled": false`
  - Disables the minimap in the editor for a cleaner workspace.
  
- **Sidebar Location**:
  - `"workbench.sideBar.location": "right"`
  - The sidebar is positioned on the right side of the editor, aligning with user preferences.

- **C++ IntelliSense**:
  - `"C_Cpp.intelliSenseEngine": "default"`
  - IntelliSense is enabled with the default engine for enhanced code completion, syntax highlighting, and error detection.
  
- **Clang Format**:
  - `"C_Cpp.clang_format_fallbackStyle": "Google"`
  - `"C_Cpp.clang_format_sortIncludes": true`
  - Clang is configured to follow the Google C++ style guide, and includes are automatically sorted.

- **Compiler Path**:
  - `"C_Cpp.default.compilerPath": "/usr/bin/g++"`
  - Sets the GCC compiler path for building and compiling C++ code in the container.

### 4. **VS Code Extensions**

The following extensions are installed to enhance the C++ development experience:

- **C++ Tools Extension Pack** (`ms-vscode.cpptools-extension-pack`): Provides debugging, IntelliSense, and code navigation for C++ projects.
- **CMake Tools** (`ms-vscode.cmake-tools`): Adds support for building and debugging C++ projects using CMake.
- **Clangd** (`llvm-vs-code-extensions.vscode-clangd`): Provides enhanced diagnostics and completion for projects using Clang.
- **GitHub Copilot** (`GitHub.copilot`): AI-assisted coding to help with code completion and suggestions.
- **GitHub Copilot Chat** (`GitHub.copilot-chat`): AI-powered chat support to help with coding tasks and queries within the editor.

### 5. **Post-Creation Commands**

After the container is initialized, the following tools are installed:

- **GCC and G++**: The GNU Compiler Collection for compiling and building C++ projects.
- **GDB**: The GNU Debugger for debugging C++ applications.
- **CMake**: A cross-platform tool for managing the build process of projects.
- **Clang and Clang-Tidy**: Alternative C++ compiler and static analysis tools for catching bugs early.
- **Clang-Format**: Tool to automatically format code according to style guidelines.
- **Valgrind**: A memory debugging tool used to detect memory leaks and other runtime errors.

### 6. **Build and Debug Tools**

This development environment is equipped with the following tools for building and debugging C++ code:
- **GCC/G++** for compilation.
- **CMake** for project build configuration.
- **GDB** for debugging.
- **Clang tools** for static analysis and formatting.

## How to Use the Development Environment

1. **Codespace Setup**: When you open this repository in GitHub Codespaces, the container will be automatically built using the settings in `devcontainer.json`. This includes installing necessary tools and extensions for C++ development.
2. **Build Projects**: Use CMake or traditional Makefile workflows to build your C++ applications.
3. **Debugging**: You can debug your C++ projects using GDB directly in VS Code, with full support for breakpoints and variable inspection.
4. **AI Assistance**: GitHub Copilot is enabled to assist you with code suggestions and completions. Copilot Chat is available for interacting with AI directly inside your editor for help with code questions and tasks.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

