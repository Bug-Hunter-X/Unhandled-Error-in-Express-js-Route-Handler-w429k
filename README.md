# Unhandled Error in Express.js Route Handler
This repository demonstrates a common error in Express.js applications: missing error handling in route handlers.  The `bug.js` file shows a route that is vulnerable to crashes if an invalid user ID is provided. The `bugSolution.js` file demonstrates a more robust solution.

## Problem
The `bug.js` file showcases a route handler that fetches user data based on an ID passed in the request parameters.  It lacks proper error handling for scenarios where the user ID is invalid (e.g., not a number, not found in the database).  This leads to unpredictable behavior, including crashes or internal server errors (500).

## Solution
The `bugSolution.js` demonstrates how to gracefully handle potential errors.  It includes error handling using `try...catch` blocks, providing more robust behavior and informative error responses to the client.