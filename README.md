#  Mini Shell Project

The **Mini Shell** project is a **C-based** command-line shell designed to provide an **interactive environment** for **executing commands**. It supports **built-in commands**, **external commands**, **job control**, **signal handling**, and **pipelining**, demonstrating expertise in **process management** and **system programming**.

---

## 🛠 Project Features

- **Command Execution:** Supports both **built-in** and **external commands**.
- **Pipelining:** Executes multiple commands **connected with pipes** (|).
- **Job Control:** Manages **background** and **foreground processes**.
- **Signal Handling:** Handles **SIGINT (Ctrl+C)** and **SIGTSTP (Ctrl+Z)** for **process control**.
- **Custom Prompt:** Allows users to **customize** the **shell prompt**.

---

## 🧰 Technology Stack

- **Programming Language:** C
- **System Programming:** Forking, Exec, Pipelining, Signals
- **Process Control:** **Job management** and **signal handling**
- **Input Handling:** Reads and **parses user input** for **command execution**
- **Error Handling:** Validates **commands**, **file operations**, and **process management**

---

## 🔄 Project Workflow

1. **User Input Handling:** Reads and **processes commands** from the **terminal**.
2. **Command Classification:** Differentiates between **built-in** and **external commands**.
3. **Command Execution:**
   - Executes **built-in commands** directly.
   - Uses **fork()**, **execvp()**, and **wait()** for **external commands**.
4. **Job Management:**
   - Supports **background execution** with **&**.
   - Implements **fg**, **bg**, and **jobs** commands for **job control**.
5. **Signal Handling:**
   - Manages **SIGINT** and **SIGTSTP** for process **termination** and **suspension**.

---

## 📂 File Structure

- `main.c` - **Initializes the shell** and manages the **main program loop**.
- `scan_input.c` - **Handles user input** and **parsing**.
- `get_command.c` - Extracts and **validates commands** from input.
- `check_command_type.c` - Distinguishes **built-in** from **external commands**.
- `execute_internal_command.c` - Executes **built-in commands** like **cd**, **pwd**, **exit**.
- `execute_external_command.c` - Manages **external commands** and **pipelining**.
- `extract_external_commands.c` - Loads **external commands** from files.
- `jobs.c` - Implements **job control** features.
- `signal_handler.c` - Handles **signals** like **SIGINT** and **SIGTSTP**.
- `main.h` - Contains **global declarations**, **function prototypes**, and **structures**.

---

## 🚀 Future Enhancements

- **I/O Redirection:** Add support for **<**, **>**, **>>** operators.
- **Command History:** Implement **storing** and **recalling previous commands**.
- **Environment Variables:** Enable **setting** and **using shell variables**.
- **Scripting Support:** Allow **execution of shell scripts**.
- **Auto-Completion:** Introduce **tab-based command completion**.

---

## 📧 Contact

For any questions, feel free to reach out:

- **Vivek**
- Email: [gopivivek57@gmail.com](mailto:gopivivek57@gmail.com)
- LinkedIn: [Vivek](https://www.linkedin.com/in/vivek57/)

