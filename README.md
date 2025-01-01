# Uncontrolled Re-renders in React's useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook and how to fix it.

## Problem

The `useEffect` hook, when used without a dependency array, runs after every render. This can lead to infinite loops, especially when the effect modifies state or props that trigger re-renders.

## Solution

To fix this, include an empty dependency array `[]` to run the effect only once after the initial render.  Alternatively, include dependencies so it runs based on specific value changes.