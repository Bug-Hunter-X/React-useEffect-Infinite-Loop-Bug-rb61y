# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications involving the `useEffect` hook.  The example shows how a missing dependency array can lead to an infinite render loop, significantly impacting performance. The solution demonstrates the proper use of the dependency array to resolve the issue.

## Bug
The `bug.js` file contains a component that uses `useEffect` without specifying any dependencies. This causes the effect to run after every render, leading to an infinite loop.

## Solution
The `bugSolution.js` file provides a corrected version. The dependency array `[count]` ensures the effect only runs when the `count` state variable changes.