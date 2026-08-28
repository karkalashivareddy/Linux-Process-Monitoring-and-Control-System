# Linux Process Monitoring and Control System

> **Operating Systems & System Programming (OSSP) Project**

**Team No.: 12**

## Team Members

| Roll No.   | Name                |
| ---------- | ------------------- |
| 2520030105 | Karkala Shiva Reddy |
| 2520030040 | Dakur Manoj Kumar   |

---

## 1. Project Overview

The **Linux Process Monitoring and Control System** is a Linux-based system programming project developed to provide a structured command-line interface for monitoring and controlling running processes.

The project demonstrates core Operating Systems concepts by interacting with the Linux `/proc` filesystem, Linux/POSIX interfaces, system calls, file descriptors, file I/O, process management mechanisms, and signals.

The system is designed to retrieve relevant information about running processes and provide controlled process-management operations using their Process IDs (PIDs).

---

## 2. Objectives

The primary objectives of the project are to:

* Monitor running processes in a Linux environment.
* Retrieve and display process information using the `/proc` filesystem.
* Inspect individual processes using their PIDs.
* Demonstrate Linux file I/O and file-descriptor usage.
* Pause and resume processes using Linux signals.
* Gracefully terminate processes when appropriate.
* Forcefully terminate processes when required.
* Demonstrate practical Linux/POSIX system-programming concepts.
* Analyze system behavior using debugging and system-call tracing tools.

---

## 3. Core Functionality

The system is designed to support the following operations:

### Process Monitoring

* List running processes.
* Display process IDs (PIDs).
* Display process names and states.
* Display parent process information.
* Retrieve CPU-related information.
* Retrieve memory-related information.

### Process Control

Processes can be selected using their PID and controlled through appropriate Linux signals:

| Operation            | Signal    | Purpose                                 |
| -------------------- | --------- | --------------------------------------- |
| Pause                | `SIGSTOP` | Suspends process execution              |
| Resume               | `SIGCONT` | Continues a stopped process             |
| Graceful Termination | `SIGTERM` | Requests controlled process termination |
| Forceful Termination | `SIGKILL` | Immediately terminates a process        |

---

## 4. Operating Systems Concepts

The project provides practical implementation and demonstration of:

* Process management
* Process identification using PIDs
* Process states
* Parent-child process relationships
* Linux `/proc` filesystem
* File descriptors
* File input/output
* Linux/POSIX system calls
* Linux signals
* Permission and error handling
* System-call tracing
* Debugging of system-level programs

---

## 5. Technology Stack

### Programming

* **C Programming Language**

### Operating Environment

* **Ubuntu/Linux**

### Build & Compilation

* **GCC**
* **GNU Make**

### Development & Debugging

* **Visual Studio Code**
* **GDB**
* **strace**

### Version Control

* **Git**
* **GitHub**

---

## 6. System Architecture

The project follows a simple command-line system-programming architecture:

```text
User
 │
 ▼
Command-Line Interface
 │
 ├── Process Discovery
 │      │
 │      └── Linux /proc Filesystem
 │
 ├── Process Inspection
 │      │
 │      └── Process Information
 │
 └── Process Control
        │
        └── Linux Signals
             ├── SIGSTOP
             ├── SIGCONT
             ├── SIGTERM
             └── SIGKILL
```

The `/proc` filesystem provides process information, while Linux/POSIX interfaces and signals provide the mechanisms required for process interaction and control.

---

## 7. Development Approach

The project development follows these stages:

1. Design the command-line interface.
2. Identify and enumerate running processes.
3. Read relevant process information from `/proc`.
4. Display process information in a structured format.
5. Implement PID-based process selection.
6. Implement process-control operations using Linux signals.
7. Add appropriate error and permission handling.
8. Compile and test the application on Ubuntu/Linux.
9. Debug the implementation using GDB.
10. Analyze system calls using strace.
11. Document implementation details and testing results.

---

## 8. Project Documentation

| File            | Description                                                               |
| --------------- | ------------------------------------------------------------------------- |
| `README.md`     | Project overview, architecture, technologies, and development information |
| `ABSTRACT.docx` | Official OSSP Team 12 project abstract                                    |

---

## 9. Expected Outcome

The expected outcome is a functional command-line application capable of monitoring Linux processes and performing controlled process-management operations.

The completed project will demonstrate practical understanding of Operating Systems and Linux system programming through direct interaction with the `/proc` filesystem, Linux/POSIX interfaces, file I/O, system calls, process management, and signals.

The project will also be supported by source code, testing evidence, documentation, screenshots, and demonstration results as development progresses.

---

## 10. Project Status

**Current Status:** Project documentation and OSSP abstract prepared.

The implementation, testing, screenshots, performance observations, and final demonstration materials will be incorporated as the project progresses.

---

## 11. Repository

**GitHub Repository:**
https://github.com/karkalashivareddy/Linux-Process-Monitoring-and-Control-System
