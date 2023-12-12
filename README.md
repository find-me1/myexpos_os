My OS Project - eXpOS (In Progress - currently working on stage21)
I'm currently working on developing an operating system using Project eXpOS, an educational platform tailored for undergraduates. Following the detailed roadmap, I'm gradually building a small OS from scratch.
                                                                                        <------------------>
Support tools : A cross compiler for an enriched XSM assembly language called the System Programming Language (SPL)  , An interface software called the XFS interface ,A cross compiler for a tiny high level programming language called the Experimental Language (ExpL).

1.we write the OS modules in the SPL language from the host (Linux/Unix) environment and generate XSM target programs using the SPL compiler.
2.The xfs-interface tool allows you to transfer executable kernel modules from your host (Linux/Unix) system to specified blocks of the XSM disk. Thus, you can load the XSM target modules into the appropriate areas of the XSM disk.
3.The ExpL compiler translates your program into the target executable format recognized by eXpOS. These programs can be stored in the XSM machine's disk using the XFS interface tool.

OS programmer's viewpoint:
            ![image](https://github.com/find-me1/myexpos_os/assets/136995186/6554d03c-0d85-4db8-8e8d-293394807839)
Application programmer's perspective:
            ![image](https://github.com/find-me1/myexpos_os/assets/136995186/9006a904-a104-449a-9cf5-93b41b6853cb)


                                                                                         <------------------>
In this project i am working on different stages (there are a total of 27 stages):

Stage1 to Stage 12 : Preparatory Stages:  The preparatory stages helps to get familiarized with the disk bootstrap loading process, disk access mechanism, file-system specification, debugger, paging hardware, interrupt handling mechanism, program loading, library linkage and function calling conventions, application binary interface (ABI), context switching between applications and so forth.

Stage13 to Stage19 : Intermediate Stages : In these stages, I have come across more advanced hardware features like, disk interrupt handling and exception handling. I have implemented some basic kernel subsystems that will be used throughout the project. I have modularized kernel into functional subsystems for resource management, memory management, device management, etc. I have implemented a primitive user interface (Shell) and the final version of the OS loader (Exec system call).

stage20 to stage27 : Final Stages: I have implemented all the system calls stipulated in the ABI documentation.I have implemented basic system calls for process creation and termination – Fork, Exec and Exit in twentieth stage. The next two stages take up system calls implementing signals and semaphores. The next three stages address the implementation of the file system. The subsequent stages add multi-user support and virtual memory support.
                                                                                          <------------------>
High Level Design of eXpOS:
          ![image](https://github.com/find-me1/myexpos_os/assets/136995186/d2375e92-5cde-4065-ad21-323a5d5ebe1a)
