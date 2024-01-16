*What is an OS*
> An operating system (OS) is system software that manages computer hardware, software resources, and provides common services for computer programs.
> It allows us to use the Low Level APIs to interact with various components of the computer.
> It also helps in managing the resources of the computer: CPU Scheduling, Memory Management, I/O devices, etc.

Types of OS:
- Uni-programming OS: Only one program can be executed at a time. 
  - > CPU is not used efficiently as the CPU is idle most of the time.
  - > CPU utilization is very low.
  - > Example: MS-DOS, ATM machines OS, Smartwatches OS, etc.
- Multiprogramming OS: Multiple programs can be executed at a time.
- > CPU is used efficiently as the CPU is not idle most of the time. 

> Can be further classified based on:
1. > No. of users: Single-user OS (Personal Computers), Multi-user OS (Mainframes/Servers)
2. > Program scheduling: Preemptive OS & Non-preemptive OS
- Multiprocessor OS: Multiple processors can be used to execute multiple programs at a time. Example: Parallel Computing in Supercomputers.

*What is a Kernel*
> The kernel is a computer program at the core of a computer's operating system with complete control over everything in the system.
> It is the first program loaded on start-up (after the bootloader) and manages the rest of the system.
> It is responsible for memory management, process management, device management, system calls, etc. and is the bridge between applications and the actual data processing done at the hardware level.

*What is a Shell*
> A shell is a user interface for access to an operating system's services.
> In general, operating system shells use either a command-line interface (CLI) or graphical user interface (GUI), depending on a computer's role and particular operation.
> It is a program that takes commands from the keyboard and gives them to the operating system to perform.
> When you open a terminal window on your Linux desktop, you are talking to the shell.
> There are different flavors of shells, but the most popular one is called bash (Bourne Again SHell) which is the default on most Linux distributions.

Some of the most popular shells are:
- bash: Bourne Again SHell - default on most Linux distributions
- zsh: Z SHell - default on macOS
- fish: Friendly Interactive SHell - default on some Linux distributions
- cmd: Windows Command Prompt - default on Windows
- powershell: Windows PowerShell - default on Windows
- command.com: MS-DOS Shell - default on MS-DOS (Microsoft Disk Operating System)

*What is a Terminal*
> A terminal is a program that opens a window and lets you interact with the shell.
> It is a program that lets you send commands to your computer and receive text-based output.
> It is a command-line interface to the shell.

*What is a CLI*
> A command-line interface (CLI) processes commands to a computer program in the form of lines of text.
> The program which handles the interface is called a command-line interpreter or command-line processor.
> Operating systems implement a command-line interface in a shell for interactive access to operating system functions or services.

*What is a Process*
> A process is an instance of a computer program that is being executed.