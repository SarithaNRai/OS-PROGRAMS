. Design, develop and implement a C/C++/Java program to simulate the working of
Shortest remaining time and Round Robin (RR) scheduling algorithms. Experiment with
different quantum sizes for RR algorithm.
Description:
Shortest remaining time (SRTF): If a new process arrives with CPU burst length less than
remaining time of current executing process, pre-empt. This scheme is known as the Shortest
Remaining-Time-First (SRTF). If a new process arrives with a shorter burst time than
remaining of current process, then schedule new process. Further reduces average waiting time
and average response time.
Round Robin scheduling algorithm (RR):
1. The queue structure in ready queue is of First in First Out (FIFO) type.
2. A fixed time is allotted to every process that arrives in the queue. This fixed time is
known as time slice or time quantum.
3. The first process that arrives is selected and sent to the processor for execution. If it is
not able to complete its execution within the time quantum provided, then an interrupt is
generated using an automated timer.
4. The process is then stopped and is sent back at the end of the queue. However, the state
is saved and context is thereby stored in memory. This helps the process to resume from
the point where it was interrupted.
5. The scheduler selects another process from the ready queue and dispatches it to the
processor for its execution. It is executed until the time Quantum does not exceed.
6. The same steps are repeated until all the process are finished.
The round robin algorithm is simple and the overhead in decision making is very low. It is the
best scheduling algorithm for achieving better and evenly distributed response time. 1.
Completion Time: Time at which process completes its execution.
2. Turn Around Time: Time Difference between completion time and arrival time.
Turn Around Time = Completion Time – Arrival Time
3. Waiting Time (W.T): Time Difference between turnaround time and burst time.
Waiting Time = Turn Around Time – Burst Time
Algorithm:
Step1: Start the process
Step2: Get the number of elements to be inserted
Step3: Get the value for burst time for individual processes
Step4: Get the value for time quantum
Step5: Make the CPU scheduler go around the ready queue allocating CPU to each process
for the time interval specified
Step6: Make the CPU scheduler pick the first process and set time to interrupt after quantum.
And after it's expiry dispatch the process
Step7: If the process has burst time less than the time quantum then the process is released
by the CPU
Step8: If the process has burst time greater than time quantum then it is interrupted by the
OS and the process is put to the tail of ready queue and the schedule selects next process from
head of the queue
Step9: Calculate the total and average waiting time and turnaround time
Step10: Display the results
Step11: Stop the process
