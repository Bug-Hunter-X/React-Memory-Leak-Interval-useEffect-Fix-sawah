# React Memory Leak with setInterval in useEffect

This repository demonstrates a common React bug involving memory leaks due to the improper use of `setInterval` within the `useEffect` hook. The bug occurs because the `setInterval` function is not properly cleaned up, leading to a continuous increase in the count and eventually a memory leak. 

The solution shows how to correctly use `setInterval` with a cleanup function to resolve the memory leak.

## Bug
The `bug.js` file demonstrates the flawed usage of `setInterval`. 

## Solution
The `bugSolution.js` file shows how to fix the bug by adding a cleanup function within the `useEffect` hook to clear the interval when the component unmounts.