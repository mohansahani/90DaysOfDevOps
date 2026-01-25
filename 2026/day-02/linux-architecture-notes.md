* The core components of Linux (kernel, user space, init/systemd)
  > There are few core concepts in linux which are the most imprtant part of linux.
  1- Kernel- Kernel is the heart of Linux operating system, it interact direcly with hardware and produce the outout throughh shell. e.g we as a user interact with application which could
    be terminal also known as shell and shell interact with kernel and gives the output. Kernel has different mechanism of understanding, its written in C programming language and understand
    only binaries no (100110).

   2- User Space provide a safe and controlled environment for running applications. It ensures that each application operates independently and securely,
    with the kernel overseeing and managing critical operations through a well-defined system call interface.

  3- init/systemd - init (short for initialization) and systemd are both system and service managers in Linux operating systems. They are the first process started by the kernel during the boot process (assigned Process ID 1, or PID 1)
  >   and are responsible for bringing the system to a usable state and managing services throughout its operation. 

* How processes are created and managed?
  > Everything in linux is a process, Every process in Linux, except the initial init or systemd process (PID 1), is created by another process.
    This forms a tree-like structure that the pstree command can visualize.
  
* What systemd does and why it matters?
  > Systemd is the default, modern init system and service manager for most Linux distributions,
  acting as the first process (PID 1) that boots the user space and manages system services (daemons), device management, and login sessions
