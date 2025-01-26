# Unhandled AsyncStorage Errors in React Native

This repository demonstrates a common error in React Native applications involving AsyncStorage: the lack of proper error handling during asynchronous storage operations.  The `bug.js` file showcases the problematic code, while `bugSolution.js` provides a corrected version with comprehensive error handling.

## Bug
The original code lacks `try...catch` blocks to handle potential errors during `AsyncStorage.setItem` and `AsyncStorage.getItem`.  This can lead to crashes or unexpected behavior if AsyncStorage operations fail.

## Solution
The solution involves wrapping the AsyncStorage calls within `try...catch` blocks. This allows for graceful handling of errors, preventing crashes and providing feedback to the user.