*What are Threads*


*Process vs Threads*
--------------------
| Process |	Thread |
--------------------
| Processes use more resources and hence they are termed as heavyweight processes. | Threads share resources and hence they are termed as lightweight processes. |
| Creation and termination times of processes are slower. | Creation and termination times of threads are faster compared to processes. |
| Processes have their own code and data/file. | Threads share code and data/file within a process. |
| Communication between processes is slower. | Communication between threads is faster. |
| Context Switching in processes is slower. | Context switching in threads is faster. |
| Processes are independent of each other. | Threads, on the other hand, are interdependent. (i.e they can read, write or change another thread’s data) |
| Eg: Opening two different browsers. | Eg: Opening two tabs in the same browser. |
--------------------
