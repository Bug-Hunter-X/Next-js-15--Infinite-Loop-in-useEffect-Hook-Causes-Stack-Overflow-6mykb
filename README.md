# Next.js 15: Infinite Loop in useEffect Hook

This repository demonstrates a common error in Next.js 15 applications involving an infinite loop within the `useEffect` hook. The `useEffect` hook, when improperly used, can lead to unexpected behavior and crashes.

## The Problem

The `about.js` file contains a `useEffect` hook that attempts to update the `count` state variable within its own dependency array. This creates an infinite loop, as the component continuously re-renders, leading to a stack overflow error. 

## Solution

The `aboutSolution.js` file provides a corrected version of the component that addresses the infinite loop. The solution involves ensuring that the dependency array for the `useEffect` hook is set up correctly, preventing the component from continuously updating itself.