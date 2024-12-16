# Unhandled Promise Rejection in Node.js HTTP Server

This repository demonstrates a common error in Node.js where an unhandled promise rejection occurs in an HTTP server due to improper error handling in asynchronous operations.  The server might crash or send incomplete responses.

## Bug Description
The provided `bug.js` file contains a Node.js HTTP server that simulates an asynchronous operation.  If this operation fails, the error is not properly handled, leading to an unhandled promise rejection.  This is a critical issue because it can cause the server to become unstable and potentially lead to unexpected behavior.

## Solution
The `bugSolution.js` file demonstrates the correct way to handle this situation.  The solution properly catches any errors that might occur within the asynchronous operation and gracefully handles them, preventing the unhandled promise rejection.

## How to Reproduce
1. Clone this repository.
2. Navigate to the repository directory.
3. Run `node bug.js` to reproduce the error.
4. Observe the error messages in the console.
5. Run `node bugSolution.js` to see the corrected behavior.

This example highlights the importance of robust error handling in Node.js applications, particularly those involving asynchronous operations.