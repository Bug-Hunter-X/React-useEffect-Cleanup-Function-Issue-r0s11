# React useEffect Cleanup Function Issue

This repository demonstrates a common issue related to the cleanup function in React's `useEffect` hook.  Improper cleanup can lead to memory leaks or unexpected side effects when a component unmounts.

## Problem:
The provided `MyComponent` uses `useEffect` without proper cleanup.  While this example is relatively benign, similar issues can lead to memory leaks, especially when dealing with subscriptions, timers, or event listeners.

## Solution:
The solution includes a corrected version with a properly implemented cleanup function that handles unmounting gracefully. This ensures that any resources acquired within the effect are released when the component is removed from the DOM.