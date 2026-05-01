Course Registration System
CSCI 230 – Data Structures & Algorithms
Tuskegee University

Team Members:

* Charles Ellis
* Andy Mohammed
* Sam O'Bryant IV

---

Project Description
This project implements a console-based course registration system that allows users to manage courses and student enrollment. The system supports adding and removing courses, registering students, dropping students, viewing course rosters, and managing waitlists. When a course reaches capacity, additional students are placed into a waitlist and are automatically promoted when a spot becomes available.

The system simulates real-world registration behavior by ensuring fairness, preventing duplicate enrollments, and maintaining consistency between course rosters and student schedules.

---

How to Compile and Run

1. Open a terminal or command prompt.

2. Navigate to the project directory containing all `.java` files.

3. Compile all files:
   javac *.java

4. Run the program:
   java Main

5. Follow the on-screen menu to interact with the system.

---

Data Structure Justification

This project uses multiple custom data structures to efficiently manage different aspects of the system:

1. Hash Map (CustomHashMap)
   A custom hash map is used to store and retrieve courses by course code. This allows for fast lookup operations with average O(1) time complexity. It ensures that course access during registration and search operations is efficient.

2. Linked List (StudentLinkedList)
   A custom linked list is used to store enrolled students and student schedules. Linked lists allow dynamic insertion and removal without shifting elements, making them ideal for frequently changing course rosters.

3. Queue (Queue<T>)
   A queue is used to manage course waitlists. The FIFO (First-In, First-Out) structure ensures fairness by enrolling students in the order they joined the waitlist when spots become available.

4. Node Structure (Node<T> and HashNode)
   Nodes are used to build the linked list and hash map structures. This reinforces understanding of how data structures are implemented at a low level without relying on built-in Java collections.

5. Service Layer (Enrollment)
   The Enrollment class acts as a helper/service layer that coordinates interactions between students and courses. This improves modularity by separating business logic from data storage.

---

Key Features

* Add and remove courses
* Register and drop students
* Automatic waitlist management
* Prevent duplicate enrollment
* View course rosters and student schedules
* Search for students within a course

---

Notes

* All data structures are implemented manually without relying on built-in Java collections (except where required for graph traversal or basic utilities).
* The system is designed for demonstration purposes and runs entirely in the console.

---

End of README
