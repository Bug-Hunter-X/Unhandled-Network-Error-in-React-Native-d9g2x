# Unhandled Network Error in React Native

This repository demonstrates a common issue in React Native applications: unhandled network errors. The provided code fetches data from an API endpoint.  The initial implementation lacks proper error handling, leading to app crashes or unhelpful error messages when the network request fails. The solution implements comprehensive error handling to improve the user experience.

## Bug

The `bug.js` file contains the buggy code.  The primary issue is the lack of robust error handling within the `useEffect` hook's asynchronous operation. If the network request fails (due to network issues, server errors, or an invalid API endpoint), the application's behavior is unpredictable; it may crash or show an unhelpful error message to the user.

## Solution

The `bugSolution.js` file offers a solution. It incorporates a `try...catch` block to gracefully handle network errors. Additionally, a `finally` block ensures the loading state is always updated, regardless of whether the request was successful or not. The error message is more informative and user-friendly.

This improved error handling leads to a more robust and user-friendly application.