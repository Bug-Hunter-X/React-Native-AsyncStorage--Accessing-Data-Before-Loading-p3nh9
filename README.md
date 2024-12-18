# React Native AsyncStorage Data Loading Issue

This repository demonstrates a common issue in React Native applications when using AsyncStorage: accessing data before it's fully loaded. The bug leads to undefined values being used, causing unexpected behavior and potentially crashes.

The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version that uses useEffect and a loading state to handle asynchronous data loading gracefully.

## How to reproduce the bug

1. Clone the repository.
2. Run `npm install`.
3. Run the app using `npx react-native run-android` or `npx react-native run-ios`.
4. Observe the initial render; you'll likely see an error or unexpected behavior due to the undefined AsyncStorage data.

## Solution

The solution utilizes the useEffect hook and a loading state to ensure the data is fetched and available before rendering the component. This prevents errors and improves the user experience.