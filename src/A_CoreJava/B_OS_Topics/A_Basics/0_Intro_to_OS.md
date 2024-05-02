### What is an OS?
> An operating system (OS) is system software that manages computer hardware, software resources, and provides common services for computer programs.
> It allows us to use the Low Level APIs to interact with various components of the computer.
> It also helps in managing the resources of the computer: CPU Scheduling, Memory Management, I/O devices, etc.

### Types of OS
1. Uni-programming OS: Only one program can be executed at a time. 
  > - CPU is not used efficiently as the CPU is idle most of the time.
  > - CPU utilization is very low.
  > - Example: MS-DOS, ATM machines OS, Smartwatches OS, etc.
2. Multiprogramming OS: Multiple programs can be executed at a time.
  > - CPU is used efficiently as the CPU is not idle most of the time. Example: Windows, Linux, macOS, etc.
  > - Can be further classified based on:
  >  1. **No. of users:** 
  >     - Single-user OS (Personal Computers)
  >     - Multi-user OS (Mainframes/Servers)
  >  2. **Program scheduling:**
  >     - #### Non-preemptive OS: 
  >       - OS cannot interrupt a program and allocate the CPU to another program. Used when a process terminates, or a process switches from running to the waiting state. Based on priority and is executed in batches(FIFO manner).
  >         - In this scheduling, once the resources (CPU cycles) are allocated to a process, the process holds the CPU till it gets terminated or reaches a waiting state.
  >         - In the case of non-preemptive scheduling, it does not interrupt a process running CPU in the middle of the execution.
  >         - Instead, it waits till the process completes its CPU burst time, and then it can allocate the CPU to another process.
  >       - It is suitable for simple systems where there is no need for a process to be terminated before it completes its execution. Eg: Printer OS, Elevator OS, etc.
  >       - It is also suitable for real-time operating systems where the process needs to complete its execution within a specified time.
  >     - #### Preemptive OS:
  >       - OS can interrupt a program and allocate the CPU to another program, used when a process switches from running to ready state or from waiting to ready state.
  >         - It is based on priority, and it is used in time-sharing systems like a time slice, round-robin, etc.
  >         - In this scheduling, a process can be removed from the CPU, and this removal is based on priority.
  >         - If the priority of the newly arrived process is higher than the priority of the process currently being executed, the CPU will be preempted.
  >         - The resources (CPU cycles) are allocated to a process for a limited amount of time, and then it is taken from the process and given to another process.
  >       - It is also suitable for real-time operating systems where the process needs to complete its execution within a specified time.
           
3. Multiprocessor OS: Multiple processors can be used to execute multiple programs at a time. 
  - > Example: Parallel Computing in Supercomputers.

### What is a Kernel?
The kernel is a computer program at the core of a computer's operating system with complete control over everything in the system.
> - It is the first program loaded on start-up (after the bootloader) and manages the rest of the system.

It is responsible for memory management, process management, device management, system calls, etc. and is the bridge between applications and the actual data processing done at the hardware level.

### What is a Shell?

A shell is a user interface for access to an operating system's services.
> In general, operating system shells use either a command-line interface (CLI) or graphical user interface (GUI), depending on a computer's role and particular operation.
> It is a program that takes commands from the keyboard and gives them to the operating system to perform.
> When you open a terminal window on your Linux desktop, you are talking to the shell.

>Some of the most popular shells are:
   - > bash: Bourne Again SHell - default on most Linux distributions
   - > zsh: Z SHell - default on macOS
   - > fish: Friendly Interactive SHell - default on some Linux distributions
   - > cmd: Windows Command Prompt - default on Windows
   - > powershell: Windows PowerShell - default on Windows
   - > command.com: MS-DOS Shell - default on MS-DOS (Microsoft Disk Operating System)

### What is a Terminal?
A terminal is a program that opens a window and lets you interact with the shell.

It is a program that lets you send commands to your computer and receive text-based output.

It is a command-line interface to the shell.

### What is a CLI?
A command-line interface (CLI) processes commands to a computer program in the form of lines of text.

The program which handles the interface is called a command-line interpreter or command-line processor.

Operating systems implement a command-line interface in a shell for interactive access to operating system functions or services.
