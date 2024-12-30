# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook. The initial implementation causes unnecessary re-renders due to an improperly used dependency array. The solution showcases the correct usage of dependency arrays to optimize component performance.

## Bug

The `bug.js` file contains a component that uses the `useEffect` hook without specifying a dependency array. This results in the effect running after every render, leading to potential performance issues. Note that this bug could cause performance degradation for complex components or with frequent updates.  This example is simple for demonstration purposes.

## Solution

The `bugSolution.js` file provides a corrected version.  The dependency array is added to the useEffect, so that it only runs when the count changes.

## How to reproduce the bug:
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server. 
4. Observe the console logs to show the useEffect running more frequently than necessary in the initial implementation (bug.js)
5. See the improved performance (less frequent log entries) and behavior in bugSolution.js
