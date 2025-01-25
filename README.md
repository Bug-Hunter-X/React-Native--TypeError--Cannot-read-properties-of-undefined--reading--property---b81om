# React Native: TypeError: Cannot read properties of undefined (reading 'property')

This repository demonstrates a common React Native error and its solution. The error, `TypeError: Cannot read properties of undefined (reading 'property')`, occurs when attempting to access a property of an object that is currently `undefined` or `null`. This often happens when dealing with asynchronous operations like fetching data from an API.

## Problem

The `bug.js` file showcases the incorrect approach where a component tries to access a property of a state variable before the state is properly updated with fetched data. This leads to the error when the component initially renders.

## Solution

The `bugSolution.js` file presents the solution using optional chaining (`?.`) and nullish coalescing (`??`). These operators provide safe ways to handle potential null or undefined values without causing the error.  Additionally, it includes a loading state to provide better user feedback while data is being fetched.