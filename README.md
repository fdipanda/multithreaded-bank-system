# multithreaded-bank-system
A C# console application demonstrating thread-safe bank account operations using multithreading and synchronization.

## Overview
This project is a **multi-threaded banking system simulation** implemented in C#.  
It demonstrates how to safely manage shared resources using **thread synchronization** to prevent race conditions.

Multiple threads perform deposits and withdrawals on shared bank accounts while maintaining data consistency through mutual exclusion.

## Concepts Demonstrated
- Multithreading in C#
- Thread synchronization using `lock`
- Critical sections and shared state protection
- Concurrent access to shared resources
- Object-oriented design

## Technologies Used
- **Language:** C#
- **Concurrency:** `Thread`, `lock`
- **Domain:** Systems Programming / Concurrency

## Project Structure
- `BankAccount` manages account balance with thread-safe operations
- `Bank` manages multiple accounts
- `Program` handles user input and spawns threads for transactions

## How It Works
1. Users create bank accounts with an initial balance
2. Deposit and withdrawal requests are executed in separate threads
3. Access to the account balance is synchronized using a lock
4. The system prevents inconsistent updates caused by concurrent access

## How to Run
```bash
dotnet run
```

Follow the console prompts to create accounts and perform transactions.

## Example Behavior
- Multiple deposits and withdrawals can occur concurrently
- Balance updates remain consistent due to synchronization
- Invalid operations (e.g., insufficient funds) are handled safely

## Academic Context
This project was developed to practice:
- Multithreaded programming
- Mutual exclusion and synchronization
- Safe handling of shared mutable state

## Author
Franck Dipanda
