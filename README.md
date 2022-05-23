# OS-Scheduler
Part I: Process Generator (Simulation &amp; IPC) Code File: process_generator.c The process generator should do the following tasks: • Read the input files (check the input/output section below). • Ask the user for the chosen scheduling algorithm and its parameters, if there are any. • Initiate and create the scheduler and clock processes. • Create a data structure for processes and provide it with its parameters. • Send the information to the scheduler at the appropriate time (when a process arrives), so that it will be put it in its turn. • At the end, clear IPC resources. Part II: Clock (Simulation &amp; IPC) Code File: clk.c The clock module is used to emulate an integer time clock. This module is already built for you. Part III: Scheduler (OS Design &amp; IPC) Code File scheduler.c The scheduler is the core of your work, it should keep track of the processes and their states and it decides - based on the used algorithm - which process will run and for how long. You are required to implement the following THREE algorithms: 1. Preemptive Highest Priority First (HPF). 2. Shortest Job First (SJF). 3. Round Robin (RR).  The scheduling algorithm only works on the processes in the ready queue. (Processes that have already arrived.) The scheduler should be able to: 1. Start a new process. (Fork it and give it its parameters.) 2. Switch between two processes according to the scheduling algorithm. (Stop the old process and save its state and start/resume another one.) 3. Keep a process control block (PCB) for each process in the system. A PCB should keep track of the state of a process; running/waiting, execution time, remaining time, waiting time, etc. 4. Delete the data of a process when it gets notifies that it finished. When a process finishes it should notify the scheduler on termination, the scheduler does NOT terminate the process. 5. Report the following information (a) CPU utilization. (b) Average weighted turnaround time. (c) Average waiting time. (d) Standard deviation for average weighted turnaround time. 6. Generate two files: (check the input/output section below) (a) Scheduler.log (b) Scheduler.perf Part IV: Process (Simulation &amp; IPC) Code File: process.c Each process should act as if it is CPU-bound. Again, when a process finishes it should notify the scheduler on termination, the scheduler does NOT terminate the process.
