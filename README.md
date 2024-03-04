# Betonic Sort Implementation in Go

This repository contains a simple implementation of the Betonic Sort algorithm in the Go programming language.

## What is Betonic Sort?

Betonic Sort, also known as Cocktail Sort or Shaker Sort, is a variation of the Bubble Sort algorithm. It improves on the Bubble Sort by allowing the "bubbles" (the smaller or larger elements) to travel in both directions through the list, thereby potentially reducing the number of passes needed to fully sort the list.

## How to Use

To use this implementation, simply clone the repository and run the following command:

```bash
go run /example/main.go
```

This will execute the sorting algorithm on a sample array defined within the `betonicSort.go` file. Feel free to modify the array to test the algorithm with different inputs.

or

```Go
import "github.com/17HIERARCH70/betonicSort"
```
## Complexity

Let <math>p = \lfloor \log_2 n \rfloor</math> and <math>q = \lceil \log_2 n \rceil</math>.

It is evident from the construction algorithm that the number of rounds of parallel comparisons is given by <math>q(q+1)/2</math>.

It follows that the number of comparators <math>c</math> is bounded <math>2 ^{p-1} \cdot p (p+1) /2 \leq c \leq \lfloor {n/2} \rfloor \cdot q (q+1) /2 </math> (which establishes an exact value for <math>c</math> when <math>n</math> is a power of 2).

Although the absolute number of comparisons is typically higher than Batcher's odd-even sort, many of the consecutive operations in a bitonic sort retain a locality of reference, making implementations more cache-friendly and typically more efficient in practice.

## Performance

The Betonic Sort algorithm has an average time complexity of O(n^2), where 'n' is the number of elements in the array. While it is not the most efficient sorting algorithm for large datasets, it can be useful for small arrays or educational purposes due to its simplicity.

