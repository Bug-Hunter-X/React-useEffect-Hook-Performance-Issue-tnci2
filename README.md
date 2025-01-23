# React useEffect Hook Performance Issue

This repository demonstrates a common performance issue in React applications related to the `useEffect` hook. The example shows how unnecessary re-renders can be avoided by correctly specifying dependencies in the `useEffect` hook.

## Bug Description
The provided code has an `useEffect` hook that runs on every render, even though it only needs to run when the count changes.  This causes unnecessary logging and potentially impacts performance with more complex components. 

## Solution
The solution involves correctly specifying the `count` variable as a dependency in the `useEffect` hook.  This ensures that the effect only runs when the `count` value changes.