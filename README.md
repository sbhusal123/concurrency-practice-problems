# concurrency-practice-problems

# Python Concurrency Practice Exercises

Here are some programming exercises for each concurrency tool you're practicing:

## Lock
1. **Bank Account Simulation**: Simulate multiple users trying to access and update a shared bank account balance. Use a `Lock` to prevent data races while depositing and withdrawing money.
2. **Inventory Management**: Create a system where multiple threads attempt to add or remove items from an inventory. Use a `Lock` to ensure accurate stock counts.
3. **File Writing Task**: Write a program where multiple threads attempt to write to a shared log file. Use `Lock` to ensure threads write sequentially to avoid file corruption.

## RLock
1. **Recursive Function with Shared Resource**: Write a recursive function where each level of recursion requires access to a shared resource (like a counter). Use `RLock` to allow the function to re-acquire the lock.
2. **Nested Lock Simulation**: Create a simulation with two resources that depend on each other (like a printer and a scanner). Use `RLock` to avoid deadlocks when both resources are needed by the same thread.
3. **Multilevel Access Control**: Simulate a program where a thread needs to lock multiple resources to perform a task. Use `RLock` to allow it to acquire locks recursively.

## Semaphore
1. **Resource Pool**: Simulate a limited resource pool (e.g., a connection pool) that can only allow a fixed number of threads to use it at any time. Use a `Semaphore` to manage access to the pool.
2. **Thread Safe Counter**: Implement a counter that multiple threads can increment or decrement, but only a set number of threads can access it simultaneously. Use a `Semaphore` to restrict access.
3. **Car Parking System**: Simulate a parking lot with a limited number of parking spots. Use a `Semaphore` to control how many cars can enter the lot.

## Event
1. **Traffic Light Control**: Use an `Event` to simulate a traffic light where threads representing cars wait until the light turns green.
2. **File Download Notifier**: Simulate a file download where a processing thread waits until a download event occurs. Use an `Event` to notify the processor that the file is ready.
3. **Race Start Countdown**: Implement a racing game where multiple threads wait for a "start race" event. Use an `Event` to signal all threads to start at the same time.

These scenarios will give you a practical way to apply each tool while managing shared resources and controlling access among threads. Let me know if you'd like specific guidance on any of these!
