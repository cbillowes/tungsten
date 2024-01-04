#algorithms

What is dynamic programming?
?
1. A problem-solving technique that breaks down a complex problem into smaller overlapping subproblems, solving each subproblem only once and storing the solutions for reuse. 
2. It optimizes efficiency by avoiding redundant computations through techniques like memoization (top-down) or tabulation (bottom-up). 
3. Dynamic programming is particularly useful for solving optimization problems with optimal substructure and overlapping subproblems.

What is memoization?
?
1. Memoization is a technique in computer programming where previously computed results are stored and reused to optimize the performance of a function.
2. It is like having a special notebook where we write down the answers to math problems we've solved before so that we don't have to solve them again. 
3. When we see the same problem, we check our notebook first, and if we find the answer, we use it without doing the work again. 

```javascript
function fibonacciMemoized() {
  const cache = {};

  function fib(n) {
    if (n <= 1) return n;
    if (cache[n] !== undefined) return cache[n];

    const result = fib(n - 1) + fib(n - 2);
    cache[n] = result;
    return result;
  }

  return fib;
}

// Create a memoized Fibonacci function
const fibonacci = fibonacciMemoized();

// Example usage
console.log(fibonacci(5)); // Output: 5
console.log(fibonacci(10)); // Output: 55
```

```clojure
(def fibonacci-memoized
  (memoize
    (fn [n]
      (if (<= n 1)
        n
        (+ (fibonacci-memoized (- n 1)) (fibonacci-memoized (- n 2)))))))

; Example usage
(println (fibonacci-memoized 5)) ; Output: 5
(println (fibonacci-memoized 10)) ; Output: 55
```

What is tabulation?
?
1. Tabulation is a dynamic programming technique where a table is filled with solutions to subproblems in a bottom-up manner.
2. Starting from the simplest and building up to the original problem. It involves iterating through the subproblems in a structured manner and computing solutions iteratively, typically using an array or matrix. 
3. Tabulation is often more intuitive for some programmers and avoids the function call overhead associated with memoization.
4. This is like a recipe where each step is carefully followed to create the final dish, ensuring efficiency and avoiding redundancy.

```javascript
function fibonacciTabulation(n) {
  const fib = new Array(n + 1).fill(0);
  fib[0] = 0;
  fib[1] = 1;

  for (let i = 2; i <= n; i++) {
    fib[i] = fib[i - 1] + fib[i - 2];
  }

  return fib[n];
}

// Example usage
console.log(fibonacciTabulation(5)); // Output: 5
console.log(fibonacciTabulation(10)); // Output: 55

```

```clojure
(defn fibonacci-tabulation [n]
  (let [fib (make-array (inc n))]
    (aset fib 0 0)
    (aset fib 1 1)
    (loop [i 2]
      (when (< i (inc n))
        (aset fib i (+ (aget fib (- i 1)) (aget fib (- i 2))))
        (recur (inc i))))
    (aget fib n)))

; Example usage
(println (fibonacci-tabulation 5)) ; Output: 5
(println (fibonacci-tabulation 10)) ; Output: 55

```

What other applications can we use memoization for?
?
1. **Recursive Function Optimization:**
    Memoization is commonly used to optimize recursive functions by caching previously computed results, avoiding redundant calculations.
    
2. **Combinatorial Problems:**
    Problems involving combinations, permutations, or choosing elements from a set can benefit from memoization to store intermediate results and improve efficiency.
    
3. **Graph Traversal:**
     Algorithms like depth-first search (DFS) or breadth-first search (BFS) can be optimized using memoization to avoid re-exploring already visited nodes.
     
4. **String Matching:**
    Memoization can be applied to string matching algorithms, such as finding the longest common subsequence or substring, to store intermediate results during recursive computations.
    
5. **Optimization Problems:**
    Various optimization problems, such as finding the shortest path in a graph, minimizing / maximizing a function, or solving the knapsack problem, can benefit from memoization.

What other applications can we use tabulation for?
?
1. **Dynamic Programming for Optimization:**
	Tabulation is a fundamental technique for solving optimization problems by iteratively filling a table with solutions to subproblems.
	
2. **Matrix Chain Multiplication:**
    In computer science, tabulation is often used for problems like matrix chain multiplication, where optimal parenthesization is determined by filling a table.
    
3. **Longest Increasing Subsequence:**
    Tabulation can be applied to find the length of the longest increasing subsequence in an array, a common problem in computer science.
    
4. **Coin Change Problem:**
    In the coin change problem, where the goal is to make change for a given amount using the fewest coins, tabulation is used to find the optimal solution.
    
5. **Sequence Alignment:**
    Bioinformatics applications, such as sequence alignment in DNA or protein sequences, often utilize tabulation for optimal alignment calculations.
    
6. **Dynamic Time Warping:**
    In signal processing, dynamic time warping (DTW) for measuring similarity between two sequences is often implemented using tabulation.
    
7. **Resource Allocation:**
    Problems involving resource allocation, scheduling, or task assignment can be efficiently solved using tabulation
    .
8. **Parsing and Syntax Analysis:**
    In compiler design and natural language processing, tabulation can be employed for parsing and syntax analysis to build parsing tables efficiently.

