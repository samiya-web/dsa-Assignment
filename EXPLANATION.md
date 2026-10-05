# DSA Assignment - Explanation

## Q1. Stack Using Array

### Aim

To implement a Stack using an Array and perform basic operations such as PUSH, POP, PEEK and DISPLAY.

### Introduction

A Stack is a linear data structure that follows the **LIFO (Last In, First Out)** principle. This means that the element inserted last is removed first.

A real-life example of a stack is a pile of plates. The plate placed last on the top is removed first.

In an array implementation of a stack, a variable called **TOP** is used to keep track of the top element.

Initially:

    TOP = -1

This indicates that the stack is empty.

### Operations of Stack

#### 1. PUSH

The PUSH operation is used to insert an element into the stack.

Before inserting an element, the program checks whether the stack is full. If the stack is full, Stack Overflow occurs.

Otherwise, TOP is increased by one and the new element is inserted.

Example:

    PUSH(10)
    PUSH(20)
    PUSH(30)

Stack:

    30  <- TOP
    20
    10

#### 2. POP

The POP operation is used to remove the top element from the stack.

If the stack is empty, Stack Underflow occurs. Otherwise, the element at TOP is removed and TOP is decreased.

Example:

    30  <- TOP
    20
    10

After POP:

    20  <- TOP
    10

The element 30 is removed.

#### 3. PEEK

The PEEK operation displays the top element of the stack without removing it.

Example:

    30  <- TOP
    20
    10

Output:

    Top element is: 30

#### 4. DISPLAY

The DISPLAY operation displays all the elements present in the stack from TOP to the bottom.

Example:

    Stack elements are:
    30
    20
    10

### Stack Overflow

Stack Overflow occurs when we try to insert an element into a stack that is already full.

### Stack Underflow

Stack Underflow occurs when we try to remove an element from an empty stack.

### Time Complexity

| Operation | Time Complexity |
|---|---|
| PUSH | O(1) |
| POP | O(1) |
| PEEK | O(1) |
| DISPLAY | O(n) |

### Applications of Stack

- Function calls
- Recursion
- Expression evaluation
- Infix, Prefix and Postfix conversion
- Undo and Redo operations
- Browser Back button
- Parentheses matching

### Conclusion

Stack is an important linear data structure based on the LIFO principle. Using an array, operations such as PUSH, POP and PEEK can be performed efficiently.

---

# Q2. Circular Queue Using Array

### Aim

To implement a Circular Queue using an Array and perform operations such as ENQUEUE, DEQUEUE, FRONT and DISPLAY.

### Introduction

A Circular Queue is a linear data structure that follows the **FIFO (First In, First Out)** principle. This means that the element inserted first is removed first.

In a circular queue, the last position of the array is connected back to the first position. This allows the queue to reuse empty spaces created after deletion.

Two important variables are used:

- **FRONT** - Points to the first element.
- **REAR** - Points to the last element.

Initially:

    FRONT = -1
    REAR = -1

This indicates that the queue is empty.

### Operations of Circular Queue

#### 1. ENQUEUE

The ENQUEUE operation is used to insert an element into the queue.

Before insertion, the program checks whether the queue is full.

The full condition is:

    (REAR + 1) % MAX == FRONT

If the queue is not full, REAR is moved to the next position and the new element is inserted.

Example:

    ENQUEUE(10)
    ENQUEUE(20)
    ENQUEUE(30)

Queue:

    FRONT -> 10  20  30 <- REAR

#### 2. DEQUEUE

The DEQUEUE operation is used to remove an element from the front of the queue.

If:

    FRONT == -1

then the queue is empty.

Otherwise, the element at FRONT is removed and FRONT is moved to the next position.

Example:

Before DEQUEUE:

    FRONT -> 10  20  30 <- REAR

After DEQUEUE:

    FRONT -> 20  30 <- REAR

The element 10 is removed.

#### 3. FRONT

The FRONT operation displays the first element of the queue without removing it.

Example:

    FRONT -> 20  30  40 <- REAR

Output:

    Front element is: 20

#### 4. DISPLAY

The DISPLAY operation displays all the elements present in the circular queue starting from FRONT and ending at REAR.

Example:

    Queue elements are: 20 30 40

### Advantages of Circular Queue

1. It makes better use of available memory.
2. Empty positions can be reused after deletion.
3. ENQUEUE and DEQUEUE operations are efficient.
4. It avoids unnecessary shifting of elements.
5. It is useful for fixed-size data storage.

### Applications of Circular Queue

- CPU scheduling
- Round Robin scheduling
- Printer scheduling
- Buffer management
- Network data buffering
- Memory management
- Traffic management systems

### Time Complexity

| Operation | Time Complexity |
|---|---|
| ENQUEUE | O(1) |
| DEQUEUE | O(1) |
| FRONT | O(1) |
| DISPLAY | O(n) |

### Circular Queue vs Linear Queue

| Circular Queue | Linear Queue |
|---|---|
| Last position connects to first position | Last position does not connect to first |
| Reuses empty spaces | Empty spaces may remain unused |
| Better memory utilization | Comparatively less memory efficient |
| Uses circular movement | Uses linear movement |

### Conclusion

A Circular Queue is an efficient implementation of a queue that follows the FIFO principle. It solves the space wastage problem of a simple linear queue by reusing empty positions. ENQUEUE and DEQUEUE operations can be performed efficiently in O(1) time.
