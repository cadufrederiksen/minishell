# 🐚 Minishell - Building Your Own Unix Shell

![C](https://img.shields.io/badge/Language-C-blue) ![Makefile](https://img.shields.io/badge/Build-Makefile-yellow) ![Readline](https://img.shields.io/badge/Library-Readline-orange) ![Norminette](https://img.shields.io/badge/Style-Norminette-green)

The **Minishell** project aims to create a basic Unix shell, similar to **Bash**, allowing students to replicate essential functionalities of a command interpreter. This project is an opportunity to thoroughly explore system programming concepts, process management, and input/output control.

---

## 📋 Project Objective

Develop a functional Unix shell capable of:
- **Executing basic commands**, such as `ls`, `echo`, `pwd`, etc.
- **Managing environment variables**, allowing you to export, modify, and access values.
- **Handling redirections** (`>`, `>>`, `<`) and **pipes** (`|`) to connect commands.
- Implementing **built-in commands**, such as `cd`, `exit`, `env`, and `export`.
- **Responding to system signals**, such as Ctrl+C, Ctrl+D, and Ctrl+\.

This project aims to teach the fundamental concepts of system programming and reveal how a basic shell operates behind the scenes.

---

## 📚 Fundamental Concepts

- **Process Management**: creating and handling child processes using `fork()` and executing them with `execve()`.
- **Redirection and Pipes**: controlling input and output with `dup2()` and connecting chained commands with pipes.
- **Signal Handling**: managing interruptions, such as Ctrl+C, to ensure the shell's stability.
- **Readline Library**: interactive command reading and history management.
- **Environment Variables**: manipulating global variables used by processes in the Unix system.

---

## ✨ Implemented Features

### 🔧 Built-In Commands
1. **`echo`**: displays a message in the terminal, with support for the `-n` flag.
2. **`cd`**: changes the current directory to the specified one.
3. **`pwd`**: displays the current working directory.
4. **`export`**: adds or modifies environment variables.
5. **`unset`**: removes environment variables.
6. **`env`**: displays all available environment variables.
7. **`exit`**: terminates the shell with an exit code.

### ⚙️ Additional Features
- **Execution of External Commands**: searches for commands in the `$PATH` and executes binary programs.
- **Support for Redirections**:
  - `>`: redirects standard output to a file.
  - `>>`: appends standard output to the end of a file.
  - `<`: redirects standard input from a file.
- **Pipes (`|`)**: connects the output of one command to the input of another.
- **Command History**: allows navigation and reuse of previous commands using the **Readline** library.
- **Signal Handling**:
  - Ctrl+C: interrupts the current command without closing the shell.
  - Ctrl+D: terminates the shell if no input is provided.
  - Ctrl+\: disabled to prevent unintended terminations.

---

## 🛠️ Tools and Standards

| Tool/Standard         | Description                                               |
|-----------------------|-----------------------------------------------------------|
| **GIT**               | Version control system to organize code development.      |
| **Makefile**          | Automates compilation and executable generation.          |
| **Norminette**        | Ensures compliance with the 42 coding style standards.      |
| **Readline Library**  | Used for interactive command input and command history.   |

---
