# React Native FlatList: Stale Data Display with Dynamic Updates

This repository demonstrates a common bug in React Native's `FlatList` component when dealing with complex data and dynamic updates.  The issue arises from inefficient key management, leading to stale data being displayed.

The `bug.js` file showcases the problematic implementation, and `bugSolution.js` provides a solution by implementing an effective key extraction strategy.

## Bug Description

When the nested property of an item changes, the `FlatList` doesn't re-render correctly due to the key remaining unchanged, leading to stale data being displayed. 

## Solution

The solution is to use a unique key that accounts for changes in nested properties.