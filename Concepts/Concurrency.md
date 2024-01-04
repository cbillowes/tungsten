#concurrency #concepts #terminology 

What is concurrency?
?
Concurrency refers to the ability of a system to execute multiple tasks or processes simultaneously, allowing overlapping and interleaved execution. In a concurrent system, different parts of a program or multiple independent programs can make progress independently, even if they are executed at the same time.

What are the key concepts related to concurrency?
?
1. **Parallelism:** While concurrency involves tasks making progress independently, parallelism specifically refers to the simultaneous execution of multiple tasks to improve overall performance.
2. **Threads:** Concurrency is often implemented using threads, which are smaller units of execution within a process. Multiple threads can run concurrently within a single process, sharing the same resources.
3. **Processes:** Concurrency can also be achieved through multiple processes, where each process has its own memory space and resources. Processes run independently and communicate with each other through inter-process communication mechanisms.
4. **Synchronization:** In concurrent systems, synchronization is essential to manage access to shared resources and prevent conflicts that may arise when multiple tasks try to access or modify the same data simultaneously.
5. **Concurrency vs. Parallelism:** While these terms are related, concurrency emphasizes tasks making progress independently, whereas parallelism focuses on tasks executing simultaneously for improved performance.

What are the trade-offs of concurrency?
?
Concurrency is crucial in modern computing, especially in systems with multiple cores or processors. It allows for efficient utilization of resources, improved responsiveness, and better overall system performance. However, managing concurrency also introduces challenges, such as race conditions, deadlocks, and the need for synchronization mechanisms to ensure the correctness of the program.

