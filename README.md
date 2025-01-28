# React useEffect Hook with Incorrect Dependencies

This repository demonstrates a common mistake when using the `useEffect` hook in React.  The provided code snippet shows an `useEffect` that runs on every render instead of only when its dependencies change, leading to unintended consequences and potential performance issues.  The solution demonstrates the correct usage of the `useEffect` hook with the appropriate dependencies in the dependency array to fix this problem.

## Bug

The original code has an `useEffect` hook that lacks the correct dependency array which causes the `console.log` statement to run on every render cycle,  causing unnecessary re-renders and potential performance problems.

## Solution

The solution correctly includes `count` in the dependency array (`[count]`).  This ensures that the `useEffect` hook only runs when the value of `count` changes.