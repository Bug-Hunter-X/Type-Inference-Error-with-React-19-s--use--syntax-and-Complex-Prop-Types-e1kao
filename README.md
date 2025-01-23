# React 19 Type Inference Bug with Complex Props

This repository demonstrates a bug related to type inference in React 19 when using the new `use` syntax with components that have complex prop types (unions or intersections).  The bug manifests as unexpected type errors or runtime exceptions, particularly when props are conditionally rendered based on component state or other props. 

## Bug Description
The issue arises due to the type checker's inability to accurately infer types within conditional logic when using complex prop types. This can lead to false positive type errors or runtime failures.

## Reproduction Steps
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console errors or unexpected behavior in the browser.

## Solution
The solution involves explicitly defining the type of the prop within the conditional rendering logic, or refactoring the prop type to be simpler and easier for the type checker to handle.  The solution also showcases how to handle asynchronous operations within the component, which are often involved in complex prop scenarios.