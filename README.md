# Firebase onAuthStateChanged Race Condition

This repository demonstrates a common race condition encountered when using Firebase's `onAuthStateChanged` listener.  The listener may not fire immediately after successful authentication, leading to UI elements displaying incorrect data.

The `authBug.js` file shows the problem. The `authSolution.js` file provides a solution using promises to ensure the authentication state is checked before UI updates.