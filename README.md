# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook:  an infinite loop caused by a missing dependency array.  The `useEffect` hook runs after every render, causing a continuous update cycle. The solution shows how to fix this by correctly specifying the dependencies.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console output and the rapid updates to the counter.

## Solution

The solution provided fixes the infinite loop by adding `count` to the dependency array of `useEffect`. This ensures the effect only runs when the `count` value changes.