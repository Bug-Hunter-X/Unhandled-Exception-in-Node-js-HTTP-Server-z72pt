# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: unhandled exceptions within HTTP servers.  Improper error handling can lead to server crashes and unexpected behavior.  The `bug.js` file showcases this issue, while `bugSolution.js` provides a corrected version with robust error handling.

## Problem

The `bug.js` file creates an HTTP server that throws an uncaught exception.  This causes the server to terminate abruptly without gracefully handling the error or notifying clients.

## Solution

The `bugSolution.js` file addresses this by implementing a `try...catch` block to handle potential exceptions.  This prevents the server from crashing and allows for logging or other actions to address the error effectively.  In a production environment, consider adding more sophisticated error handling, such as sending an error response to the client or alerting monitoring services.