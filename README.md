# Task_Executor

1.	The solution provides an implementation of the provided TaskExecutor interface. 
2.	The TaskExecutor accepts and executes implementations of the provided Task interface.
3.	The TaskExecutor and Task interface implements the definitions given in the source files including package and exact method signatures i.e. no changes to the interfaces are made. 
4.	Each thread is assigned a unique name when created. See Thread.setName(String). 
5.	Threads are maintained in a pool and reused to execute multiple Tasks. Threads are not created and destroyed for each task’s execution. 
6.	Tasks executes concurrently on N threads where N is the thread pool size and is provided as a service initialization parameter. 
7.	When the number of tasks exceeds the number of threads, unexecuted tasks remain on the FIFO until removed by a unassigned thread. 
8.	Every thread’s execution blocks when the FIFO is empty i.e. Threads do not spin or busy-wait when attempting to obtain a task from the service’s empty FIFO. 
9.	The deliverable is a library jar file which is be linked with the test applications used to initialize and test the TaskExecutor’s correct implementation. 
10.	The TaskExecutor catches, report (log), and eat any exceptions thrown during an application-specific Task’s execution i.e. an exception should not cause a thread to exit. 
