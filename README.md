# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router Dom v6.  The problem occurs where other routes are defined and function correctly, but the catch-all route fails to catch any unexpected paths.  The solution provided addresses this by ensuring the catch-all route is placed correctly within the route hierarchy. 

## Steps to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to a non-existent route. You'll find the catch-all route is not triggered. 

## Solution

The solution involves correctly placing the catch-all route at the end of the route definitions to ensure it acts as a true fallback.