# LRU-page-fault

Experiment name : Least Recently Used (LRU) Page Replacement Algorithm

Introduction :
The Least Recently Used (LRU) page replacement algorithm is a fundamental technique used in operating systems to manage memory efficiently. It ensures that the most recently accessed pages remain in memory while replacing the least recently used ones.
In this lab report, we analyze and explain an implementation of the LRU algorithm in C. The provided code simulates memory management using a fixed number of memory frames.

Code Overview:

Objective:
Simulate memory management using the LRU algorithm.
Track page requests and manage available memory frames.

Code Components:
incomingStream: An array representing a sequence of page requests.
frames: The number of available memory frames.
queue: An array to store pages currently in memory.
distance: An auxiliary array to track distances of pages from their last occurrence.
occupied: The count of occupied memory frames.
pagefault: The total number of page faults.

Algorithm Steps:
For each incoming page request:
Check if the page is already in memory (hit).
If not, handle the page fault:
If frames are available, add the page to memory.
Otherwise, replace the least recently used page (LRU).
Update the queue and distance arrays accordingly.


Output:
The program prints the incoming pages and the memory state after each request.
It also reports the total number of page faults.

Conclusion
The LRU algorithm strikes a balance between simplicity and efficiency. While straightforward to implement, it may not always be optimal. Other algorithms like FIFO or optimal page replacement can provide different trade-offs.
