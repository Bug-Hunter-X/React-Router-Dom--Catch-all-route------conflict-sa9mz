# React Router Dom: Catch-all Route Conflict

This repository demonstrates a common issue with React Router's catch-all route (`/*`). When used incorrectly, it can conflict with other, more specific routes, leading to unexpected behavior where the catch-all route always matches, overriding intended routing.

## Problem:

The catch-all route should be used as the last route in your `Routes` component. If placed before more specific routes, it will always match, effectively rendering other routes unreachable.

## Solution:

The solution is to ensure that the catch-all route (`/*`) is declared *after* all other specific routes in your routing configuration.