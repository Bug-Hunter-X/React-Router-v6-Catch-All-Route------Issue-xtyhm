# React Router v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router v6.  The catch-all route, intended to handle 404 errors, is unexpectedly overriding other defined routes.

The issue is that the `/*` route matches *all* paths, including those already matched by other more specific routes. This prevents other routes from rendering properly.

**Solution:**  The provided solution shows how to resolve this by correctly ordering routes and using the `useLocation` hook for dynamic route handling.