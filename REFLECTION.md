# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:I discovered that multithreading enables several threads to run simultaneously within a single program throughout this project. I realized that Java classes that extend the Thread class or implement Runnable can be used to construct threads. I gained knowledge about how threads can transition between various thread states, including New, Runnable, Running, Waiting, and Terminated. The CPU scheduler determines which thread runs next, therefore it was unexpected to learn that threads do not always run in the order they are initiated. Additionally, I learnt about synchronization and the need of avoiding race situations when several threads share resources**

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:figuring out each process's wait and turnaround times. I initially struggled to comprehend how to manage processes with the same priority and maintain consistency in the sequence of execution. Testing the program with various sets of procedures to ensure that all edge cases functioned properly presented another challenge. Debugging the code when the output did not match expectations was also difficult for me, particularly for larger input instances. I gained a better understanding of operating system scheduling algorithms and the significance of accuracy in managing several processes at once thanks to this assignment.**

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:I overcome these difficulties by decomposing the issue into manageable chunks. In order to comprehend the reasoning, I first manually computed waiting and turnaround times for a few sample processes. I then gradually put the computations into code, testing each modification to make sure it was accurate. To learn more about sorting arrays and utilizing comparators for priority scheduling, I consulted internet resources including the Java documentation. Additionally, I created debug statements to monitor each process's execution, which enabled me to swiftly find and correct mistakes. In order to make it easier to test and debug methodically, I finally divided my code into several functions for sorting, calculating times, and printing results.**

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:Many real-world applications that require tasks to execute concurrently without interfering with the main program use multithreading. Web browsers, for instance, use several threads to simultaneously load webpages, execute scripts, and play videos. Threads are used in games to manage user input, physics calculations, and graphics rendering all at once. Threads are frequently used by mobile apps to manage background operations, such as data downloads or notification sending, while maintaining a dynamic user interface. Programs can increase responsiveness and performance by utilizing multithreading, which is precisely what I saw when I simulated process scheduling for this project. It made it easier for me to see why operating systems and apps use threads to effectively handle multiple tasks at once.**

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?
I'd like to know more about advanced concurrency ideas like thread pools, locks, semaphores, and the low-level scheduling implemented by operating systems. Additionally, I'm interested in how memory management and multithreading interact, as well as how to avoid deadlocks in large systems.
[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?
I consider myself to be Intermediate. I know how to start threads, control how they run, and deal with simple synchronization. Implementing scheduling logic in programs such as this assignment gives me confidence. I still need to practice handling deadlocks, optimizing multithreaded programs for practical uses, and advanced concurrency approaches, too.

[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
