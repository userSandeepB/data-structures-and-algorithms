# Data Structures

Data structure is a particular way of storing abd organizing data in a computer so that it can be used efficiently. A data structure is a special format for organizing and storing data. General data structure types include arrays, files, linked lists, stacks, queues, trees, graphs and so on.

Depending on the organization of the elements, data structures are classified into two types:

1. **Linear data structures**: Elements are accessed in a sequential order but it is not compulsory to store all element sequentially. Examples: Linked Lists, Stacks and Queues.

2. **Non - linear data structures**: Elements of this data structure are stored/accessed in a non-linear order Examples: Trees and graphs.

# Big O

Imagine we have multiple implementation of the same function (problem), how can we determine which one is the best? and Thats really Big O is about.

> Write a function that calculates the sum of all numbers from 1 up to some number n.

```javascript
// Implementation 1: Complexity O(n)
function addUpTo(n) {
  let total = 0;
  for (let i = 1; i <= n; i++) {
    total += i;
  }

  return total;
}
```

```javascript
// Implementation 2: Complexity O(1)
fucnton addUpTo(n) {
    return n * (n + 1) / 2;
}
```

**Big O Notation allow us to talk formally about how the runtime of an alogrithm grows as the input grows.**

### Simplifying Big O Expression

- O(2n) --> O(n)
- O(500) --> O(1)
- O(13n<sup>2</sup>) --> O(n<sup>2</sup>)
- O(n + 10) --> O(n)
- O(100n + 50) --> O(n)
- O(n<sup>2</sup> + 5n + 8) --> O(n<sup>2</sup>)

### Big O Shorthand

1. Arithmetic operations are constant
2. Variable assignment is constant
3. Accessing elements in an array (by index) or object (by key) is constant
4. In a loop, the complexity is the length of loop times the complexity of whatever happens inside the loop
