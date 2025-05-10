# CCU-Oeration-System-LAB

## Introduction
There are lab's assignments for the operating system course at National Chung Cheng University.  

## Tools:   
1.FreeRTOS

![FreeRTOS](https://github.com/wengjiahuang0529/CCU-Oeration-System-LAB/blob/0a994589553a58285a0226ace790005dd4d54799/picture/FREERTOS.png)


2.NUC140      
![NUC140](https://github.com/wengjiahuang0529/CCU-Oeration-System-LAB/blob/8d136fdfd919d4b20a434c203b51f3d856e42000/picture/NUC-140.png)

## LAB1:
**Description:**

A, B, C, and D are four students attending Mr. Warren's class together. One day, Mr. Warren decides to have them call out their names at regular intervals. A calls out every seven seconds, B every three seconds, C every two seconds, and D every five seconds. 

**Requirements:**
* A, B, C, and D each represent a task.
* At 0 seconds, all four students will simultaneously call out for the first time.
* Please provide a screenshot showing the situation from the 100th to the 110th second.

## LAB2
**Description:**

There is a toilet with two compartments available for use. Students A, B, C, and D need to use the toilet periodically. A cleaner regularly closes the toilet for cleaning.

**Requirements:**
* Implement 6 tasks: Student A, B, C, D, Cleaner, and a task responsible for displaying time.
* Use the concept from the Readers-Writers Problem.
* Implement a function to handle cleaning the toilet (similar to the writer in Readers-Writers).
* Implement another function to handle students using the toilet (similar to the reader in Readers-Writers).
* There are two compartments in the toilet for students to use alternately.
* The cleaner must wait until no student wants to use the toilet before starting cleaning.
* During cleaning, students cannot use the toilet.
* Protect the count of students using the toilet (count++ / count--) with a mutex.

## LAB3
**Description:**

Four philosophers, A, B, C, and D, are seated around a circular dining table, and they have only two activities: thinking or eating.

There are four chopsticks on the table, with one placed between each pair of adjacent philosophers. When a philosopher wants to eat, they first pick up the chopstick on their left. After picking up the left chopstick, they pause briefly before picking up the right chopstick. Only when they have both chopsticks can they start eating. After finishing their meal, they return the chopsticks.

Each chopstick can only be used by one person at a time. If a chopstick is already taken, the philosopher must wait until it is returned.

**Requirements:**
* Use 4 LEDs on the development board to represent philosophers A, B, C, and D.
* A LED lit indicates that the philosopher is eating.
* A LED off indicates that the philosopher is thinking, resting, or waiting for utensils.
* Philosophers are normally in the "Thinking" state and don't need to do anything.
* Pressing each of the 4 keypads triggers philosopher A, B, C, or D to enter the "hungry" state.
* Pressing Keypad 1 → Philosopher A wants to eat.
* Pressing Keypad 2 → Philosopher B wants to eat... (similarly for philosophers C and D)
* When in the "hungry" state, there are four stages:
* State 1: Waiting for the left chopstick.
* State 2: Rest for 500ms.
* State 3: Waiting for the right chopstick.
* State 4: Eating for 1000ms.

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/WJH910529/CCU-Oeration-System-LAB)
