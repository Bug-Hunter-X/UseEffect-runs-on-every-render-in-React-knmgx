# React useEffect Runs on Every Render

This repository demonstrates a common issue in React where the `useEffect` hook runs on every render instead of only when its dependencies change.  The example shows how to correctly use `useEffect` to avoid unnecessary re-renders and potential performance issues.

## Problem

The provided code includes a `useEffect` hook without specifying any dependencies or specifying it incorrectly. This means the effect runs after every render of the component, leading to potential performance problems and unintended side effects.  In this case, it logs "Count changed" to the console on every render, even though the console log is not strictly necessary for the application to function correctly.

## Solution

The solution correctly specifies the dependency array `[count]` for the `useEffect` hook.  Now, the effect only runs when the `count` value changes.  This significantly improves the performance of the application and avoids unnecessary computations or side effects.

## How to run

1. Clone this repository.
2. Navigate to the repository's directory in your terminal.
3. Run `npm install` to install the necessary dependencies.
4. Run `npm start` to start the development server.
