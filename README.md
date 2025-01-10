# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The bug is caused by a missing dependency in the useEffect's dependency array.  This leads to an infinite loop of renders. 

## Bug Description
The provided `MyComponent` uses `useEffect` to log the count. Because `count` is not included in the dependency array, the effect runs after every render, causing an infinite loop.  The solution corrects the dependency array to include count.