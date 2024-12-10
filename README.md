# Expo CLI: Deceptive 'Unexpected Identifier' Error with Vector Icons

This repository demonstrates a common, yet deceptively tricky, error encountered when using Expo's `@expo/vector-icons` package. The problem arises when attempting to import a specific icon set (like FontAwesome5) without having installed the corresponding package.

## The Problem
The error message is often vague, simply indicating an 'Unexpected identifier', providing little guidance.  This makes identifying the root cause challenging for developers, especially those new to Expo.

## Reproduction
The `bug.js` file illustrates the faulty code.  Observe that FontAwesome5 icons are imported, but the necessary package isn't installed.  Trying to run this code will lead to the 'Unexpected identifier' error.

## Solution
The `bugSolution.js` file presents the corrected approach.  Ensure you install the relevant icon set package using `expo install @expo/vector-icons@13.0.0 @expo/vector-icons@12.0.0` before importing. 

This clear explanation and accompanying code examples help developers quickly understand and resolve this common, yet elusive, Expo CLI issue.