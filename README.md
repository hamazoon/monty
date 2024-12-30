# Monty

This repository contains an interpreter for the Monty ByteCode language. Monty ByteCode is a simple stack-based language that provides operations for stack manipulation, arithmetic, and more. This project demonstrates concepts such as file parsing, stack/queue management, and implementing interpreters in C.

---

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Examples](#examples)
- [Compilation](#compilation)
- [Testing](#testing)
- [Author](#author)

---

## Introduction

The **Monty** interpreter reads Monty ByteCode files (with `.m` extension) and processes commands to manipulate a stack or queue. The language supports basic stack operations, arithmetic instructions, and other utilities. This project provides an opportunity to dive into the inner workings of interpreters and stack-based execution.

---

## Features

- Supports stack and queue data structures.
- Implements Monty ByteCode instructions such as:
  - `push`: Pushes an element to the stack.
  - `pall`: Prints all elements in the stack.
  - `pint`: Prints the top element of the stack.
  - `pop`: Removes the top element of the stack.
  - Arithmetic operations: `add`, `sub`, `mul`, `div`, `mod`.
  - Stack utilities: `swap`, `rotl`, `rotr`.
  - Comments with `#`.
- Handles invalid commands gracefully with error messages.
- Modular design for extensibility.

---

## Project Structure

### Files

- **`monty.c`**: Entry point for the interpreter. Handles file reading and command execution.
- **`bytecodes/`**: Directory containing example Monty ByteCode files.
- **`opcodes.c`**: Implements stack operations (`push`, `pop`, `pall`, etc.).
- **`arithmetic.c`**: Implements arithmetic operations (`add`, `sub`, etc.).
- **`stack.c`**: Defines the stack and queue operations.
- **`utils.c`**: Helper functions for parsing and error handling.
- **`monty.h`**: Header file containing function prototypes and data structures.

---

## How It Works

1. **File Parsing**  
   The interpreter reads a Monty ByteCode file line by line and parses the commands.

2. **Instruction Execution**  
   Each command is mapped to its corresponding C function, which performs the specified operation.

3. **Error Handling**  
   The interpreter checks for syntax errors, invalid commands, and stack underflows.

---

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/hamazoon/monty.git
   cd monty

