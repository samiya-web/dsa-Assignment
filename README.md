# DSA Assignment

## Student Information

| Detail | Information |
|---|---|
| **Name** | Samiya |
| **Student ID** | BC2025525 |
| **Course** | BCA |
| **Semester** | 3rd Semester |
| **Subject** | Data Structures and Algorithms |
| **Assignment** | DSA Assignment |

---

## Q1. Stack Using Array

### Description

A stack is a linear data structure that follows the **LIFO (Last In, First Out)** principle. The element inserted last is removed first.

### Implemented Operations

- **PUSH()** – Inserts an element into the stack.
- **POP()** – Removes the top element.
- **PEEK()** – Displays the top element.
- **DISPLAY()** – Displays all stack elements.
- Stack Overflow and Underflow handling.

### Complexity

| Operation | Time Complexity | Extra Space |
|---|---|---|
| PUSH | O(1) | O(1) |
| POP | O(1) | O(1) |
| PEEK | O(1) | O(1) |
| DISPLAY | O(n) | O(1) |

Stack Overflow occurs when an element is inserted into a full stack. Stack Underflow occurs when an element is deleted from an empty stack.

---

## Q2. Circular Queue Using Array

### Description

A circular queue is a linear data structure that follows the **FIFO (First In, First Out)** principle. The last position is connected to the first position to reuse empty spaces.

### Implemented Operations

- **ENQUEUE()** – Inserts an element into the queue.
- **DEQUEUE()** – Removes an element from the queue.
- **FRONT()** – Displays the front element.
- **DISPLAY()** – Displays all queue elements.
- Queue Full and Empty handling.

### Complexity

| Operation | Time Complexity | Extra Space |
|---|---|---|
| ENQUEUE | O(1) | O(1) |
| DEQUEUE | O(1) | O(1) |
| FRONT | O(1) | O(1) |
| DISPLAY | O(n) | O(1) |

### Circular Queue vs Linear Queue

1. Circular Queue reuses empty positions of the array.
2. It reduces unnecessary space wastage.
3. ENQUEUE and DEQUEUE operations take O(1) time.
4. The last position is connected back to the first position.

---

## Files Included

| File | Description |
|---|---|
| `stack.c` | Stack implementation using array |
| `circular_queue.c` | Circular Queue implementation using array |
| `README.md` | Assignment documentation |

## Technologies Used

- C Programming
- Data Structures and Algorithms
- GitHub
