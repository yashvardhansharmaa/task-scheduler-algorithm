# Task Scheduler Algorithm

This project implements a task scheduling system in Python. It provides functionality to schedule tasks based on their priorities, durations, and dependencies. The code utilizes different data structures, including `MinHeap` and `MaxHeap` from the `heapq` package, to efficiently manage fixed and flexible tasks.

## Features
- Separate handling of fixed and flexible tasks using `MinHeap` and `MaxHeap` respectively
- Prioritization of tasks based on durations and dependencies
- Clear tracking of scheduled tasks and their start times
- Flexibility in managing both fixed and flexible tasks
- Efficient management of task dependencies

## How It Works
The task scheduler function follows a straightforward strategy. It assigns priorities to tasks based on their durations and dependencies. Fixed tasks, with predetermined start times, are scheduled first. Flexible tasks, which can be scheduled at any available time, are prioritized based on their durations using a `MaxHeap`.

The code ensures that tasks with earlier start times are scheduled first for fixed tasks. For flexible tasks, it prioritizes those with longer durations, considering both the task's own duration and the durations of its dependencies.

## Advantages and Limitations
Advantages of the code:
- Handles both fixed and flexible tasks efficiently
- Prioritizes tasks based on durations and dependencies
- Provides clear tracking of scheduled tasks
- Efficiently manages task dependencies

Limitations of the code:
- Does not consider logical event relationships or time preferences
- Lacks real-time task prioritization
- Difficulty in accurately estimating task durations
- Missing a user-friendly interface

Overall, the code provides an effective but simplified task scheduling solution.
