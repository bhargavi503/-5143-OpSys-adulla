# Chapter 2 Review Questions
Name: Adulla Bhargavi
Course: 5143 Operating Systems
Date: 16 Feb 2016 

## Question 1
What are three objectives of an OS design?
1.Convenience: An operating system helps the user to use the computer in a convinent way.
2.Efficiency: The Computer system resources can be used in an efficient manner by using the operating system.
3.Ability to evolve: An operating system should be designed in such a way to permit the effective development, testing, 
and introducing the new system functions without interfering with service.

## Question 2
What is the kernel of an OS?
In computing,kernel is known as the central component of operating system.
The kernel acts as the bridge between the applications and actual data processing which is done at the harware level.
The kernel is a part of operating system that helps us to access the system resources.
It manages the file system and set interrupts for the CPU and enables the multitasking.

## Question 3
What is multiprogramming?
Multiprogramming is a form of parallel processing in which several programs can run at a time in a uniprocessor.
since we have the single processor we cannot execute all the different programs simultaneously.
Instead of that the operating system executes a part of one program,then the other part of different program and so on it continues.
For the user it appears like all the programs are executing at a time.

## Question 4
What is a process?
In the computing environment,the process is called as an instance of computer program that is being executed.
This computer program is a collection of instructions and process is the actual execution of those instructions.
If there are several instances for a single program that means more than one process is executed.

## Question 5
How is the execution context of a process used by the OS?
Also known as process state in the execution context,it is the internal data in operating system and uses to control or supervise the process.

## Question 6
List and briefly explain five storage management responsibilities of a typical OS?
Automatic allocation and management:
This the process where the allocation should be transfered to the software programmer.
Protection and access control:
This is the procedure of sharing memory , when sharing is required by a specific application it likewise debilitates the integrity of programs.
Long term storage:
Even the computer is swicthed off the memory is stored for a longer period in the RAM.
Support of modular programming:
It supports the program to define programs modules , create, destroy and alter the size of modules dynamically.
Process isolation:
It helps in prevention of data interfering from the each other process isolation.

## Question 7
Explain the distinction between a real address and a virtual address?
real address
1.It is a number that specifics a page in the memory that a hardware can address.
2.The real address is provided by the hardware.
3.The valid addresses are usually in a range of 0 to maximum value specified by the machine.
4.It is divided into fixed called as pages
virtual address.
1.It is a number within the address space of given program that corresponds to a real address.
2.The virtual address is provided by the OS kernel.
3.This may start with zero ,but not necessarily.
4.It is divided into fixed size called as frames.

## Question 8
Describe the round-robin scheduling technique?
During the execution of the process the CPU uses the round robin scheduling algorithm.
This round robin algorithm is a pre-emptive algorithm similar to the first come first serve scheduling algorithm.
In order to schedule all the process equally,round robin employs the time-sharing and gives each job a time slot and
interrupts the job if not executed in that particular time slot.
This job is resumed next time with the another time slot assigned by that process.
If the process terminates or changes its state then the schedular selects the first process in the queue ready to execute.

## Question 9
Explain the difference between a monolithic kernel and a microkernel?
Memory management:
In Mono kernel everything is processed in the kernel space. 
In the Micro kernel it only contains the basic facilities in kernel code and remaining is done in the user space.
Security and stability:
If one of the process gets crashed in process management module then the whole system goes down in monolithic kernel.
In case of micro Kernel,the kernel will be active because most of the work is done in user address space.

## Question 10
What is multithreading?
multithreading is a process to execute multiple processes or threads concurrently in a central processing unit or a single core,
appropriately supported by the operating system.

## Question 11
List the key design issues for an SMP operating system?
Simultaneous concurrent processes or threads: Kernel routines need to be reentrant to allow several processors to execute the same kernel code simultaneously.
Scheduling: Any kind of processor may perform scheduling,so the conflicts must be avoided.
Synchronization: With multiple active processes having potential access to shared address spaces or shared I/O resources,
care must be taken to provide effective synchronization
Memory Management: Memory administration on a multiprocessor must manage the greater part of the issues found on uniprocessor machines. 
If there is a problem with the cache memories,they contain image of a portion of main memory. 

