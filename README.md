# Command Argument Passing System

## Abstract
The **Command Argument Passing System** is a C-based command-line utility designed to demonstrate process creation, execution, and synchronization in a Linux/UNIX environment. It showcases the fundamental mechanics of how a parent application transfers commands and their associated arguments to a newly created child process using core system calls like `fork()`, `exec()`, and `wait()`. The system effectively handles parsing user-provided inputs, launching requested programs with their respective argument lists, displaying the received arguments, and ensuring proper process synchronization. This project serves as a practical model for understanding the process lifecycle, inter-process execution flow, and robust error handling for invalid commands.

## Scenario
A command-line application needs to execute different programs while passing user-provided arguments to them. The system must correctly transfer the command and its arguments from the parent application to the newly executed program.

## Problem Statement
The system needs to demonstrate how processes receive command-line arguments and how a new program can be executed with those arguments seamlessly without terminating the parent application prematurely.

## Features & Tasks Implemented
This project is built in **C** and fulfills the following system requirements:
- **Input Parsing:** Accepts a command and multiple arguments from the user.
- **Process Creation:** Creates a child process using the `fork()` system call.
- **Argument Passing:** Successfully passes dynamic arguments to the child process.
- **Program Execution:** Uses an appropriate `exec()` family function (e.g., `execvp()`) to execute the requested program.
- **Argument Display:** Displays the arguments received by the new program upon execution.
- **Error Handling:** Gracefully handles invalid commands, missing files, and argument errors.
- **Dynamic Execution:** Allows different commands to be executed sequentially with different argument lists.
- **Process Synchronization:** Uses `wait()` or `waitpid()` to synchronize the parent and child processes, ensuring the parent waits for the child to finish executing before prompting for the next command.

## Technologies Used
* **Language:** C
* **OS Environment:** Linux / UNIX
* **System Calls:** `fork()`, `execvp()`, `wait()`, `waitpid()`, `exit()`

## How to Compile and Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/karkalashivareddy/Command-Argument-Passing-System.git](https://github.com/karkalashivareddy/Command-Argument-Passing-System.git)
   cd Command-Argument-Passing-System