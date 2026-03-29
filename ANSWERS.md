# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

A process is an independent program with its own memory and resources, while a thread is a smaller unit inside a process that shares the same memory.
Processes are heavier and slower to create, while threads are lightweight and faster.
Threads share data easily but need synchronization.
We used threads because they are more efficient and suitable for simulating concurrent tasks.

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

If a process does not finish within its time quantum, it is moved to the end of the ready queue.
It waits for its next turn while other processes execute.

Example from my output:
P1 executed for 2 units
P1 not finished → moved to end of queue
P2 starts execution

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

```
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
P1 used its time slice but didn’t complete, so it was re-queued.
After other processes run, P1 gets another turn later.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

New: When P1 is created but not started yet.
Runnable: When P1 is ready and waiting in the queue.
Running: When P1 is being executed by the CPU.
Waiting: When P1 is paused (e.g., waiting for its next turn).
Terminated: When P1 finishes execution completely

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. New: When P1 is created but not started yet.
2.Runnable: When P1 is ready and waiting in the queue.
3.Running: When P1 is being executed by the CPU.
4.Waiting: When P1 is paused (e.g., waiting for its next turn).
5.Terminated: When P1 finishes execution completely.

  

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

Example 1: Web Browser

Description: Handles multiple tabs at the same time.
Why Round-Robin works well here: It gives each tab a fair share of CPU time, keeping the browser responsive.

Example 2: Operating System Task Scheduling

Description: Manages multiple running programs.
Why Round-Robin works well here: Ensures fairness and prevents any process from starving.

---

## Summary

**Key concepts I understood through these questions:**
1. Difference between threads and processes
2.How Round-Robin scheduling works
3.Thread lifecycle and states
4.Importance of fairness and concurrency
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
