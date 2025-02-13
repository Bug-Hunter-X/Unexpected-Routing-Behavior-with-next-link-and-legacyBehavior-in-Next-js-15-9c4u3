# Unexpected Routing Behavior with next/link and legacyBehavior in Next.js 15

This repository demonstrates a bug encountered when using the `legacyBehavior` prop with the `next/link` component in Next.js 15. The bug manifests as unexpected routing behavior, particularly on the client-side.

## Bug Description

The `legacyBehavior` prop was introduced as a workaround for older Next.js versions, but in Next.js 15, using it can cause issues with the new routing mechanism.  Client-side navigation might not work as expected, resulting in broken links or incorrect page transitions. 

## Reproduction

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Navigate to the application and click the links. Observe the behavior and compare it with the solution.

## Solution

The recommended solution is to remove the `legacyBehavior` prop and rely on the default Next.js 15 routing behavior. This usually resolves the issue without requiring additional configuration.