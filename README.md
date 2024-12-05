# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common mistake when using the `useEffect` hook in React. The effect runs on every render, leading to performance issues and unnecessary console logs.  The solution shows how to fix it.

## Bug

The `useEffect` hook in `bug.js` lacks the correct dependency array. It runs on every render because it's missing the `[count]` dependency array which tells the hook only to run when the `count` variable changes.