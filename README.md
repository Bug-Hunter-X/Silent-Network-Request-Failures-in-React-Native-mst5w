# Silent Network Request Failures in React Native

This example demonstrates a common issue in React Native applications where network requests fail silently due to unhandled promise rejections.  The provided code lacks proper error handling within the `fetch` call, causing the application to appear unresponsive or behave unexpectedly when a network error occurs.

The solution implements robust error handling using a `try...catch` block, providing user feedback in case of a network error.  The `finally` block ensures that the loading indicator is always hidden, improving the user experience.

## How to Reproduce

1. Run the `bug.js` code.
2. Simulate a network error (e.g., by disconnecting from the internet or using a wrong API endpoint).
3. Observe that the application doesn't provide any feedback to the user about the network failure.

## Solution

The `bugSolution.js` file contains the corrected code with proper error handling and feedback for the user.
