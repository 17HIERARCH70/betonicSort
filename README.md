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

In the Bitonic Sort algorithm, let's define:

- $p = \lfloor \log_2 n \rfloor$
- $q = \lceil \log_2 n \rceil$

It's evident from the construction algorithm that the number of rounds of parallel comparisons is given by $\frac{q(q+1)}{2}$.

Therefore, the number of comparators $c$ is bounded by:

$$ 2^{p-1} \cdot p(p+1)/2 \leq c \leq \left\lfloor \frac{n}{2} \right\rfloor \cdot q(q+1)/2 $$

This establishes an exact value for $c$ when $n$ is a power of 2.



