# Chapter 3 Review Questions
Name: Daita Manjusri
Course: 5143 Operating Systems
Date: 01 02 2016

## Question 1

What does it mean to preempt a process?
Preemption is a kind of multi tasking where a particular task is interrupted without any permission from the current running task. 
This task is generally carried out by a scheduler called preemptive scheduler. It is a kind of temporary interruption.

##Question 2

What is swapping and what is its purpose?
1.Swapping is a technique used by operating system. It is used to increase the processor utilization. 
2.The blocked processes are moved into the secondary memory and a chance is given for the execution of  the newly  arrived process .
3.As the processes are moved they are called temporary suspended process. Simply saying swapping is called a memory management technique.

##Question 3

List three general categories of information in a process control block?
1.PCB is also called as process table. This table contains information in order to manage process.
2.Three general categories of information in a PCB are Process identification data ,Process control data, Process state data.
3.Process identification data contains a specific identifier. This identifier is used to cross verify the tables to know which process uses which I/o. 
4.Process state data defines status of process when suspended and lets it again execute correctly .Process control state is used to manage the process itself, it contains program counters, process state ad many more.

##Question 4

Why are two modes (user and kernel) needed?
User mode is used for the users to execute their programs. Generally user mode doesn’t have access to hardware. Kernal mode is referred as system mode . 
All processes begin execution in user mode, and they switch to kernel mode only when obtaining a service provided by the kernel. User mode can't read/write directly to OS memory. 
Kernel mode can read and write directly from OS memory. Faults in user mode results in effecting system stability but faults in kernel results in system failure.

##Question 5

What is the difference between an interrupt and a trap?
When a program is executing in a system, there can be events that could interrupt the execution flow these are called interrupts. 
These interrupts can be two types hardware and software. Hard ware interrupts are called simple interrupts and software interrupts are called traps. 
Occurrences of hardware may result in disabling of other hardware interrupts but this may not come true for traps.

##Question 6

Interrupt is generally a signal either from hardware or software. 
Interrupts are of two types hardware interrupt and software interrupt. 
Examples of interrupts are division of zero which is a software interrupt and power failure is a hardware interrupt, wrong press of key from keyboard is also a hardware interrupt .

##Question 7

Process switch is to switch the process state between  status like read , blocked, write etc.
While switch mode is to switch the process between user mode and kernel mode.
Mode switch is less expensive.Process switch is more expensive .
