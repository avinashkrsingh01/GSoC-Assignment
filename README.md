# CMake Hello World Project

This project demonstrates a basic setup for using CMake, a powerful build system generator that helps manage the build process across different platforms.

## Introduction to CMake

CMake is a tool that generates build files for various environments (such as Makefiles on macOS/Linux or Visual Studio project files on Windows) to compile code consistently across platforms. It is commonly used in C/C++ projects to simplify project configuration and building.

### Key Components of CMake

- **CMakeLists.txt**: This file is the main configuration file for CMake, where we specify information about the project, source files, and build targets.
- **Variables**: CMake allows setting variables for defining project settings (e.g., `PROJECT_NAME`, `CMAKE_MINIMUM_REQUIRED_VERSION`) and to pass options through commands.
- **Commands**: Common CMake commands include `project()` (to define the project name), `add_executable()` (to specify the output executable), and `cmake_minimum_required()` (to specify CMake version compatibility).

### How CMake Works

CMake reads the `CMakeLists.txt` file and generates platform-specific build files:
- **Makefiles** on Unix-based systems, used with `make` to compile the code.
- **Project files** for IDEs like Visual Studio or Xcode.

## Project Structure

The project consists of two files:

- `hello.c`: Contains the "Hello, World!" source code.
- `CMakeLists.txt`: Contains the CMake configuration.

### `hello.c`

```c
#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}
