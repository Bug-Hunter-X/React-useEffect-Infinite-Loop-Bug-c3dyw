# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook causing an infinite loop.  The issue arises from incorrectly specifying the dependency array, leading to unintended re-renders.  The solution showcases the correct way to manage dependencies within `useEffect` to prevent this problem.  The code uses functional components and the `useState` hook.

## Bug

The bug lies within the `useEffect` hook.  Without adding the `count` variable to the dependency array, the effect runs on every render, triggering another state update, and creating an infinite loop.

## Solution

The solution correctly includes `count` in the dependency array.  This ensures the effect only runs when `count` changes.