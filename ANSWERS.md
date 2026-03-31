# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:*A thread is a smaller unit of execution, whereas a process is an autonomous program that has its own memory space and system resources. Because each process has its own memory and context switching is more costly, creating and managing processes is more difficult. On the other hand, because they share the same memory area, threads are lightweight and have easy communication. Since the simulation requires several tasks to perform concurrently with minimal overhead, we used threads rather than processes in this assignment. The program runs more quickly and effectively when threads are used, particularly when modeling scheduling methods like Round-Robin.*

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:A process is pushed back to the end of the ready queue in Round-Robin scheduling if it does not complete within the allotted time quantum. This ensures that all programs are treated fairly by allowing other processes to receive CPU time. The procedure will wait for its turn once more before starting up again in the following cycle. This cycle keeps going till the procedure is finished.**

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output:
P1 executed for 2 units, remaining time = 3
P2 executed for 2 units, remaining time = 1
P3 executed for 2 units, remaining time = 4
P1 re-added to queue
```
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

 1 -New: When P1 is formed in the program but before the start() method is used to start the thread, it is in the New state.
Runnable: P1 enters the Runnable state, ready to run and awaiting CPU scheduling, after calling start().
2. Running: When the CPU scheduler chooses P1, it enters the Running state and begins carrying out its instructions within its time quantum.
3. Waiting: If P1 is paused, such as when it completes its time quantum and waits in the ready queue for its next turn, it may enter the Waiting state. If there are delays or synchronization issues, it can also wait.
Terminated: After finishing all of its execution, P1 enters the Terminated state (when its burst time becomes
---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1:
An explanation:
Web servers manage several client requests concurrently, including loading webpages, pictures, and data from several users.

Why Round-Robin is effective in this situation:
Round-Robin makes sure that every request receives an equal amount of CPU time and doesn't interfere with other requests. This enhances responsiveness and keeps consumers from experiencing delays. When numerous users access the server at once, it is extremely helpful.



### Example 2:
An explanation:
Operating systems oversee several concurrently running programs, such as browsers, audio players, and background services.

Why Round-Robin is effective in this situation:
By allocating a set amount of time to each activity, round-robin scheduling guarantees equity. This makes the system responsive by preventing any one application from consuming entire CPU time. For time-sharing systems where several jobs require equal attention, it is perfect.

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes and why threads are more efficient
2. How Round-Robin scheduling manages the ready queue and ensures fairness
3. The lifecycle of a thread and its different states during execution

**Concepts I need to study more:**
1. Advanced thread synchronization techniques (locks, semaphores)
2. Deadlocks and how to prevent them
