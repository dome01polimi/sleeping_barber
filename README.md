# Sleeping Barber Problem

This repository contains a C program that simulates the classic **Sleeping Barber Problem**, which is a synchronization problem in operating systems. It illustrates the coordination between barber and customers using semaphores and multithreading in C.

## Problem Description

In this simulation:
- A barber sleeps when there are no customers.
- When a customer arrives, they wake up the barber if the barber is asleep.
- If there is an available seat in the waiting room, the customer waits; otherwise, they leave.
- The barber serves one customer at a time and continues this process until all customers are served.

## Requirements

To compile and run the program, you will need:
- GCC (GNU Compiler Collection)
- pthread library (POSIX Threads)
- semaphore library (part of pthread)

## Compilation

To compile the program, navigate to the directory where the `sleeping_barber.c` file is located and use the following command:

```bash
gcc -pthread sleeping_barber.c -o sleepingbarber
