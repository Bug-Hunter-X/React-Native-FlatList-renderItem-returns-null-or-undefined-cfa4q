# React Native FlatList renderItem returns null or undefined

This repository demonstrates a common error in React Native's FlatList component where the `renderItem` function returns `null` or `undefined` under certain conditions. This leads to unexpected behavior and crashes.

The `bug.js` file shows the problematic code, and `bugSolution.js` provides the corrected version.

## Problem

The `renderItem` function in `FlatList` must always return a valid React element. If it returns `null`, `undefined`, or any other non-React element, it throws an error or causes unexpected behavior, like skipping items in the list.

## Solution

The solution is to ensure that the `renderItem` function always returns a valid React element, even when conditions are not met. This usually means returning a placeholder element or using conditional rendering with care.