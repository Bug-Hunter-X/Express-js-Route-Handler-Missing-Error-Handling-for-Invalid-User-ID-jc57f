# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of error handling for invalid input.  Specifically, the provided code attempts to access a user based on an ID provided in the URL parameters. However, it lacks proper error handling if the provided ID is not a valid integer.

The `bug.js` file contains the problematic code. The `bugSolution.js` file provides a corrected version with robust error handling.

## Bug
The `bug.js` file shows the original code with missing error handling. Attempting to access the route with a non-numeric ID will cause an error. 

## Solution
The `bugSolution.js` file demonstrates a corrected implementation. It includes error handling to gracefully handle non-numeric IDs and other potential errors, returning appropriate HTTP status codes.