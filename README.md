# React useEffect Infinite Loop Bug
This repository demonstrates a common error in React's `useEffect` hook:  an infinite loop caused by omitting the dependency array. 

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides the corrected version.

## Problem
The `useEffect` hook in `bug.js` runs after every render because the dependency array is missing.  This creates an infinite loop, causing performance issues and potentially crashing the application. 

## Solution
The `bugSolution.js` file fixes this by adding an empty dependency array `[]` to the `useEffect` hook. This ensures that the effect runs only once after the initial render, preventing the infinite loop.