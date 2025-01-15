# React Router Dom v6 Catch All Route '*' Issue

This repository demonstrates a problem encountered when using the catch-all route `*` in React Router DOM v6. The issue involves the catch-all route interfering with other defined routes, preventing them from rendering correctly.

The `App.js` file contains the buggy code, while `AppSolution.js` shows the corrected version.

## Problem

The catch-all route, intended to handle all unmatched paths, is inappropriately intercepting requests meant for other routes, leading to incorrect rendering.

## Solution

The solution involves ensuring the catch-all route is positioned correctly within the `Routes` component, preferably as the last route defined. This ensures it only handles requests that do not match any other defined route.