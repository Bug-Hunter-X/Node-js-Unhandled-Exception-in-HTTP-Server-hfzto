# Node.js Unhandled Exception Example

This repository demonstrates a common error in Node.js: unhandled exceptions within an HTTP server's request handler.  Unhandled exceptions can lead to unexpected server crashes and data loss.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version.

## Problem

The `bug.js` file throws an error in the request handler without proper error handling. This results in the server process crashing, requiring manual restarting.

## Solution

The `bugSolution.js` file demonstrates how to properly handle exceptions within the request handler using a `try...catch` block. This prevents the server from crashing and allows for graceful error handling, such as logging errors or returning an error response to the client.

## How to Run

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `node bug.js` to observe the unhandled exception.
4. Run `node bugSolution.js` to see the corrected version.