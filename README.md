# React setInterval Memory Leak
This repository demonstrates a common React bug involving memory leaks when using `setInterval` within the `useEffect` hook without proper cleanup.

The `bug.js` file shows the problematic code. The `setInterval` is started, but never stopped, leading to a memory leak when the component unmounts.

The `bugSolution.js` file provides the corrected code, demonstrating how to use `clearInterval` to prevent the memory leak.