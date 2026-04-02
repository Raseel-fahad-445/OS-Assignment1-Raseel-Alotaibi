# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[A process is an independent program with its own memory, while a thread is a smaller part inside a process that shares memory with other threads. Threads are faster to create, use fewer resources, and communication between them is easier, while processes need more complex ways to communicate.

We used threads in this project because they’re more efficient for simulating CPU scheduling. Using processes would be slower and take more resources. In SchedulerSimulation.java, each process is linked to a thread to simulate execution using Thread.start().]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[If a process doesn’t finish its time quantum, it goes back to the ready queue so other processes can get CPU time. This keeps things fair and makes sure every process gets its turn.]

Example from my output:
```
[hhhh]
```

**Explanation of example:**
[A thread goes through several states: New when created, Runnable when start() is called, Running when the CPU executes it, Waiting if it sleeps or waits, and Terminated when it’s done.
In our project, when process P1 is created, it starts as New, then start() makes it Runnable, it runs for its time quantum (Running), may sleep (Waiting), and finally finishes (Terminated). This shows how threads move through their lifecycle to manage CPU execution efficiently.
]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[A thread starts in the New state when created. When Thread.start() is called, it becomes Runnable. When the CPU executes it, it becomes Running. If Thread.sleep() is used, it goes to Waiting. Finally, when execution finishes, it becomes Terminated. In my program, each process follows these states during scheduling.]

1. **New**: [A thread starts in the New state when created. ]

2. **Runnable**: [When Thread.start() is called, it becomes Runnable]

3. **Running**: [When the CPU executes it, it becomes Running]

4. **Waiting**: [If Thread.sleep() is used, it goes to Waiting.]

5. **Terminated**: [when execution finishes, it becomes Terminated. In my program, each process follows these states during scheduling.]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Name of application/scenario]

**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2: [Name of application/scenario]

**Description**: 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: 
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

---

## Summary

**Key concepts I understood through these questions:**
1. 
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
