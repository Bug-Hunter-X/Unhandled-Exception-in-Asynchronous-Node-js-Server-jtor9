# Unhandled Exception in Asynchronous Node.js Server

This repository demonstrates a common error in Node.js: unhandled exceptions within asynchronous operations.  The server simulates an asynchronous task that randomly fails. Without proper error handling, this leads to a server crash.

## Bug
The `bug.js` file contains a Node.js HTTP server that simulates an asynchronous operation.  If the operation 'fails' (simulated randomly), an uncaught `Error` is thrown, causing the server to crash.

## Solution
The `bugSolution.js` demonstrates how to correctly handle exceptions within asynchronous operations using `try...catch` blocks. Even though errors are simulated randomly, the server remains operational.