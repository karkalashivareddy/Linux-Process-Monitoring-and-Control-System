\# Koneru Lakshmaiah Education Foundation\[cite: 1]

(Deemed to be University estd. u/s. 3 of the UGC Act, 1956)\[cite: 1]

Off-Campus: Bachupally-Gandimaisamma Road, Bowrampet, Hyderabad, Telangana - 500 043.\[cite: 1]

Phone No: 7815926816, www.klh.edu.in\[cite: 1]



\*\*OPERATING SYSTEMS AND SYSTEMS PROGRAMMING (25CS2104E)\*\*\[cite: 1]

\*\*2026–27, Term-I\*\*\[cite: 1]



\## Project Problem Statement Submission Form\[cite: 1]



\*\*Section No.:\*\* sec-3\[cite: 1]

\*\*Team No.:\*\* 12\[cite: 1]

\*\*Project Title:\*\* Command Argument Passing System



\### Team Members\[cite: 1]

| Roll Number | Student Name | Signature |

| :--- | :--- | :--- |

| 2520030105 | Karkala Shiva Reddy | |\[cite: 1]

| 2520030040 | Dakur Manoj Kumar | |\[cite: 1]



\---



\### 1. Abstract

Command-line applications often need to execute distinct programs while accurately passing user-provided arguments. This project aims to build a C-based utility in a Linux/UNIX environment that demonstrates fundamental process management and inter-process execution. The system resolves this by utilizing core POSIX system calls to parse inputs, transfer arguments, and synchronize execution. The project focuses on OS concepts such as process creation (`fork()`), program execution (`execvp()`), and parent-child synchronization (`wait()`/`waitpid()`). The proposed system will prompt the user for a command and arguments, spawn a child process, execute the requested program with the passed arguments, display the received arguments, and ensure the parent process waits for the child's completion before resuming. The expected outcome is a functional, interactive terminal application that effectively models program execution flows and handles invalid commands gracefully.



\### 2. Problem Statement

A command-line application needs to execute different programs while passing user-provided arguments to them. The system must correctly transfer the command and its arguments from the parent application to the newly executed program. A system-programming solution is required to demonstrate how processes receive command-line arguments and how a new program can be executed seamlessly without terminating the parent application prematurely. 



\### 3. Objectives

\* To build a system that accepts a command and multiple arguments from the user.

\* To create a child process using the `fork()` system call.

\* To pass dynamic arguments to the child process and execute the requested program using the `exec()` family of functions (e.g., `execvp()`).

\* To display the arguments received by the new program upon execution.

\* To synchronize the parent and child processes using `wait()` or `waitpid()`.

\* To handle invalid commands and argument errors gracefully.



\### 4. Proposed Methodology

\* The project will be developed in C Programming Language and executed in an Ubuntu/Linux environment.\[cite: 1]

\* The system will utilize a loop to continuously prompt the user for input.

\* User input will be parsed into an array of strings representing the command and its arguments.

\* The `fork()` system call will be utilized to spawn a child process. 

\* Within the child process, `execvp()` will be called to replace the child's memory space with the new program, passing the parsed argument array.

\* The parent process will invoke `wait()` or `waitpid()` to suspend its execution until the child process terminates, ensuring synchronization.

\* The system will display appropriate error messages for invalid commands or execution failures.

\* The overall flow will be: Read Input → Parse Arguments → Fork Child → Execute Program (Child) / Wait (Parent) → Report Result → Repeat.



\### 5. Operating Systems Concepts / Linux APIs Used

| OS Concept / Linux API / System Call | Purpose in the Project |

| :--- | :--- |

| \*\*`fork()`\*\* | Create a child process to run the new command. |

| \*\*`execvp()`\*\* | Execute the requested program and pass the argument list. |

| \*\*`wait()` / `waitpid()`\*\* | Synchronize the parent process to wait for the child's completion. |

| \*\*Process Management\*\* | Handling process creation, execution, and termination states. |

| \*\*String Manipulation\*\* | Parsing raw terminal input into argument arrays. |

| \*\*POSIX/Linux system calls\*\* | Provide core process-control interfaces. |



\### 6. Individual Contribution

| Roll Number | Student Name | Individual Responsibility |

| :--- | :--- | :--- |

| 2520030105 | Karkala Shiva Reddy | Implement input reading and string parsing logic; manage process creation using `fork()`; setup the GitHub repository. |

| 2520030040 | Dakur Manoj Kumar | Implement process execution using `execvp()`; handle parent-child synchronization with `wait()`; design error handling for invalid commands. |



\### 7. Tools / Platforms / Software Used

| Tool / Platform / Software | Purpose |

| :--- | :--- |

| \*\*Linux / Ubuntu\*\* | Run and test the command argument passing system. |

| \*\*C programming language\*\* | Develop the system and Linux/POSIX interfaces. |

| \*\*GCC compiler\*\* | Compile the C program. |

| \*\*Visual Studio Code\*\* | Write, organize, and edit the project source code. |

| \*\*Git and GitHub\*\* | Version control and project source-code management. |



\### 8. Expected Outcome

\* The system will allow users to input dynamic commands and multiple arguments.

\* The system will successfully spawn child processes to handle executions without crashing the parent.

\* The system will accurately pass and display arguments to the executing program.

\* The project will provide a practical understanding of fundamental OS process lifecycles, execution handoffs, and process synchronization.



\### 9. GitHub Repository

\*\*GitHub Repository Link:\*\* https://github.com/karkalashivareddy/Command-Argument-Passing-System

\*\*Repository Created:\*\* Command-Argument-Passing-System

\[X] Yes     \[ ] No



\---

\*\*Faculty Name:\*\* K HEMA\[cite: 1]

\*\*Signature:\*\* \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

\*\*Remarks:\*\* \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_



\*\*Project Approved:\*\* \[ ] Yes     \[ ] No

\*\*Date:\*\* \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

\*\*Faculty Signature:\*\* \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

