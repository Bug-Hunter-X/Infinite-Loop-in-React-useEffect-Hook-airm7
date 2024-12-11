# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving an infinite loop in the `useEffect` hook. The `useEffect` hook is used to perform side effects in functional components, but without a dependency array, it will run continuously, leading to performance problems and potentially crashing the application.

## Bug Description
The `bug.js` file contains a functional component that uses the `useEffect` hook without a dependency array. The effect increments a state variable `count` in every render cycle, creating an infinite loop.

## Solution
The `bugSolution.js` file presents a corrected version of the component. By adding an empty dependency array `[]` to the `useEffect` hook, we ensure that the effect runs only once after the initial render, preventing the infinite loop.