# DSA Assignment

**Name:** Samiya  
**Course:** BCA  
**Semester:** 3rd Semester 
**student ID:** BC2025525
**Subject:** Data Structures and Algorithms  
**Assignment:** DSA Assignment

---

## Q1. Stack Using Array

### Description

A stack is a linear data structure that follows the **LIFO (Last In, First Out)** principle.

### Implemented Operations

- PUSH()
- POP()
- PEEK()
- DISPLAY()
- Stack Overflow handling
- Stack Underflow handling

### Complexity

| Operation | Time Complexity | Extra Space |
|-----------|-----------------|-------------|
| PUSH      | O(1)            | O(1)        |
| POP       | O(1)            | O(1)        |
| PEEK      | O(1)            | O(1)        |
| DISPLAY   | O(n)            | O(1)        |

### Stack Overflow

When the stack is completely full and we try to insert another element, it is called **Stack Overflow**.

### Stack Underflow

When the stack is empty and we try to remove an element, it is called **Stack Underflow**.

---

## Q2. Circular Queue Using Array

### Description

A circular queue is a linear data structure in which the last position is connected back to the first position. It follows the **FIFO (First In, First Out)** principle.

### Implemented Operations

- ENQUEUE()
- DEQUEUE()
- FRONT()
- DISPLAY()
- Queue Full handling
- Queue Empty handling

### Complexity

| Operation | Time Complexity | Extra Space |
|-----------|-----------------|-------------|
| ENQUEUE   | O(1)            | O(1)        |
| DEQUEUE   | O(1)            | O(1)        |
| FRONT     | O(1)            | O(1)        |
| DISPLAY   | O(n)            | O(1)        |



1. Circular Queue reuses the empty positions at the beginning of the array.
2. ENQUEUE and DEQUEUE operations take O(1) time.
3. Circular Queue uses array space more efficiently.
4. Linear Queue may leave unused spaces at the beginning after deletion.
5. Circular Queue solves this problem by connecting the last position to the first position

| File | Description |
|------|-------------|
| `stack.c` | Stack implementation using array |
| `circular_queue.c` | Circular Queue implementation using array |
| `README.md` | Assignment documentation 
