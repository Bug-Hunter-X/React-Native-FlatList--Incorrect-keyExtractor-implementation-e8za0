# React Native FlatList: Incorrect keyExtractor Implementation

This repository demonstrates a common error in React Native's FlatList component: using the index as the `keyExtractor`. This can lead to unexpected behavior and performance issues.  The solution shows how to correctly implement `keyExtractor` for optimal performance and UI consistency. 

## Bug Description
Incorrectly using `keyExtractor` with the index as the key leads to issues when items are added, removed, or reordered in the list.  React Native may not update the UI correctly, resulting in stale or duplicated items.

## Solution
The solution utilizes a unique identifier from each item in the data array as the key.  This ensures that each item has a stable, unique identifier, even if the data changes.

## How to reproduce
1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the application on an emulator or physical device.
4. Observe the issues with the incorrect `keyExtractor` implementation in `bug.js`.
5. Compare with the corrected implementation in `bugSolution.js`.