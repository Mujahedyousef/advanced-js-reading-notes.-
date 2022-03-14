[Live URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_9/class_9.html)

# Read: Stacks & Queues

## 1. Stack

> Is a linear data structure in which elements can be inserted and deleted only from one side of the list, called the top.

* How to work?

> A stack follows the LIFO (Last In First Out) principle
>> The element inserted at the last is the first element to come out.
>

* Can do operations in a stack:

1. push operation : To insertion of an element into the stack.
1. pop operation : To deletion of an element from the stack.

* In stack, we always keep track of the last element present in the list with a pointer called ==top==.
![stack](/day_9/stack-1.png)

----

## 2. Queues

> Is a linear data structure in which elements can be inserted only from one side of the list called ***rear***, and the elements can be deleted only from the other side called the ***front***.

* How to work?

 > FIFO (First In First Out) principle.
 >> the element inserted at first in the list, is the first element to be removed from the list.

* Can do operations in a Queues:

1. **insertion** of an element in a queue is called an **enqueue operation**
2. **deletion** of an element is called a **dequeue operation**.

* In queue we always maintain two pointers:
>
> 1. one pointing to the element which was inserted at the first and still present  in the list with the front pointer.
> 1. Second pointer pointing to the element inserted at the last with the rear pointer.

![queue](/day_9/queue-1.png)
----

## Difference between Stack and Queue Data Structures

|  Stacks   |   Queues |
|--- |--- |
|  Stacks are based on the LIFO principle, i.e., the element inserted at the last, is the first element to come out of the list.  | Queues are based on the FIFO principle, i.e., the element inserted at the first, is the first element to come out of the list. |
| Insertion and deletion in stacks takes place only from one end of the list called the top.   | Insertion and deletion in queues takes place from the opposite ends of the list. The insertion takes place at the rear of the list and the deletion takes place from the front of the list. |
| Insert operation is called push operation.   | Insert operation is called enqueue operation. |
| Delete operation is called pop operation.   | Delete operation is called dequeue operation. |
|  In stacks we maintain only one pointer to access the list, called the top, which always points to the last element present in the list.  | In queues we maintain two pointers to access the list. The front pointer always points to the first element inserted in the list and is still present, and the rear pointer always points to the last inserted element. |
|  Stack is used in solving problems works on recursion.  | Queue is used in solving problems having sequential processing. |
----
