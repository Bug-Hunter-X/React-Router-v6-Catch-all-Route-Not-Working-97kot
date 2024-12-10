# React Router v6 Catch-all Route Issue
This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router v6. The catch-all route is intended to handle any unmatched paths, but in this case, it's always being triggered even when valid routes exist.

## Problem Description
The provided `App.js` contains a simple React Router setup with three routes: `/`, `/about`, and a catch-all route `/*`. However, regardless of the path, the NotFound component (404 page) is always rendered.

## Solution
The solution provided in `AppSolution.js` addresses this issue by reordering the routes within the `Routes` component. Placing the catch-all route as the last route resolves the conflict and ensures that the catch-all route is only invoked when no other route matches.