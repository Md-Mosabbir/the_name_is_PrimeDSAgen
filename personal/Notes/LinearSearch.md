# What is Linear Search?

Linear search is the simpliest form of search that can be performed in a data structure. We walk linearly over an array and for each element we check whether the given value matches. if it is true we return something else we return something else.

## Code Example

```typescript
export default function linear_search(
    haystack: number[],
    needle: number,
): boolean {
    for (let i = 0; i < haystack.length; i++) {
        if (haystack[i] === needle) {
            return true;
        }
    }

    return false;
}

```

As we can see we walk over each element and return true if the given value matches any element within the array. 

# Time Complexity (Big O)

As the worst case is that we walk the full lenght of the array so it is Big O of n. 


> Note: For measuring Big O we need to keep these in mind:

1. Growth is with respect to the input
2. Constants are dropped
3. Worst case is the usually the way to measure
