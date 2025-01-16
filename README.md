# React useEffect Cleanup Function Issue

This repository demonstrates a common issue with React's `useEffect` hook where the cleanup function is not called correctly on component unmount. This can lead to memory leaks, unexpected behavior, or other issues.

## Problem

The `useEffect` hook in the provided `bug.js` file includes a cleanup function, but this function isn't being executed as expected when the component unmounts. This might be due to improper use or interaction with other parts of the application.  The issue is that the effect runs only once on mount, and the console log for unmount never happens, indicating that the cleanup function is not being invoked.

## Solution

The solution, found in `bugSolution.js`, addresses this by ensuring that the cleanup function executes correctly, which is vital for managing side effects and avoiding potential problems.