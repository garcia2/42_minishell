# Minishell

**Minishell** is a project from 42 school that involves creating a basic Unix shell. The goal is to develop a functional shell that can interpret and execute commands, manage processes, and handle system calls.

## Table of Contents
1. [Overview](#overview)
2. [Project Architecture](#project-architecture)
3. [Technologies Used](#technologies-used)
4. [Features](#features)
5. [Installation](#installation)
6. [Usage](#usage)
7. [Author](#author)

## Overview

The **Minishell** project is a simplified implementation of a Unix shell that supports basic commands, input/output redirections, and pipes. This project is designed to provide experience with process management, signals, and how shells interpret and execute commands.

## Project Architecture

- **Command Parsing** : Parses user input to handle commands, options, and arguments.
- **Process Management** : Uses `fork()`, `execve()`, and `wait()` system calls to create and manage child processes.
- **Signal Handling** : Catches and manages signals (e.g., Ctrl+C) to control shell behavior.

## Technologies Used

- **C Language** : Core language for shell implementation
- **Unix System Calls** : For process management, input/output, and signal handling

## Features

1. **Basic Command Execution** : Execute basic system commands found in Unix.
2. **Input and Output Redirection** : Supports `<`, `>`, and `>>` for redirection of input and output.
3. **Piping** : Ability to use pipes (`|`) to chain multiple commands together.
4. **Environment Variables** : Access and modify environment variables within the shell.
5. **Signal Handling** : Manages signals for interruption and suspension (e.g., Ctrl+C, Ctrl+Z).

## Installation

To set up `minishell`, clone the repository and compile the program.

```bash
git clone https://github.com/garcia2/42_minishell
cd 42_minishell
make
```

This will create an executable named `minishell`.

## Usage

To run the shell, execute the following command:

```bash
./minishell
```

Once running, you can enter commands as you would in a standard Unix shell. Some examples:

- Run simple commands: `ls`, `echo "Hello"`
- Use redirections: `echo "Hello" > output.txt`
- Chain commands with pipes: `cat file.txt | grep "text"`

## Author

Project developed by [Nicolas Garcia](https://github.com/garcia2) as part of 42 school.
