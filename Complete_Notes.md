# Chapter 1: The Foundations - Logic and Proofs
# 1.1 Propositional Logic
Propositions
A proposition is a declarative sentence that is either true or false, but not both

Denoted by propositional variables: p, q, r, s, ...

Truth values: True (T) or False (F)

Logical Operators
Operator	Name	Notation	True when
¬	Negation	¬p	p is false

∧	Conjunction	p ∧ q	Both p and q are true

∨	Disjunction	p ∨ q	At least one is true (inclusive or)

⊕	Exclusive or	p ⊕ q	Exactly one is true

→	Conditional	p → q	p false or q true

↔	Biconditional	p ↔ q	p and q have same truth value

Conditional Statements
Hypothesis: p, Conclusion: q

Ways to express p → q:

"if p, then q"

"p implies q"

"p only if q"

"p is sufficient for q"

"q is necessary for p"

"q unless ¬p"

Converse: q → p

Contrapositive: ¬q → ¬p (equivalent to original)

Inverse: ¬p → ¬q

Precedence of Logical Operators
¬ (highest)

∧

∨

→

↔ (lowest)

# 1.2 Applications of Propositional Logic
System specifications: Translating requirements into logical expressions

Consistency: No conflicting requirements that lead to contradictions

Boolean searches: AND, OR, NOT operators for web searches

Logic puzzles: Knights (always truth) and knaves (always lie)

# 1.3 Propositional Equivalences
Types of Compound Propositions
Tautology: Always true

Contradiction: Always false

Contingency: Neither tautology nor contradiction

Logical Equivalences (p ≡ q means p ↔ q is a tautology)
Law	Formula

Identity	p ∧ T ≡ p, p ∨ F ≡ p

Domination	p ∨ T ≡ T, p ∧ F ≡ F

Idempotent	p ∨ p ≡ p, p ∧ p ≡ p

Double negation	¬(¬p) ≡ p

Commutative	p ∨ q ≡ q ∨ p, p ∧ q ≡ q ∧ p

Associative	(p ∨ q) ∨ r ≡ p ∨ (q ∨ r), (p ∧ q) ∧ r ≡ p ∧ (q ∧ r)

Distributive	p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r), p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r)

De Morgan's	¬(p ∧ q) ≡ ¬p ∨ ¬q, ¬(p ∨ q) ≡ ¬p ∧ ¬q

Absorption	p ∨ (p ∧ q) ≡ p, p ∧ (p ∨ q) ≡ p

Negation	p ∨ ¬p ≡ T, p ∧ ¬p ≡ F

Conditional Equivalences
p → q ≡ ¬p ∨ q

p → q ≡ ¬q → ¬p

p ↔ q ≡ (p → q) ∧ (q → p)

Satisfiability
A compound proposition is satisfiable if there exists an assignment of truth values that makes it true

Unsatisfiable if false for all assignments

# 1.4 Predicates and Quantifiers
Predicates
Predicate: Statement P(x) involving variable x

Becomes a proposition when values are assigned

Quantifiers
Quantifier	Notation	Meaning	True when

Universal	∀x P(x)	P(x) for all x	P(x) true for every x

Existential	∃x P(x)	There exists x such that P(x)	P(x) true for at least one x

Uniqueness	∃!x P(x)	There exists exactly one x	P(x) true for exactly one x

Negating Quantifiers (De Morgan's Laws for Quantifiers)

¬∀x P(x) ≡ ∃x ¬P(x)

¬∃x P(x) ≡ ∀x ¬P(x)

Binding Variables
Bound variable: Within scope of a quantifier

Free variable: Not bound by quantifier

# 1.5 Nested Quantifiers
Order Matters!
∀x∃y P(x,y): For every x, there exists a y (y may depend on x)

∃y∀x P(x,y): There exists a y such that for all x (y is independent)

Translating Mathematical Statements
"The sum of two positive integers is positive": ∀x∀y((x>0) ∧ (y>0) → (x+y>0))

Fallacies
Affirming the conclusion: (p → q) ∧ q → p (not valid)

Denying the hypothesis: (p → q) ∧ ¬p → ¬q (not valid)

# 1.7 Introduction to Proofs
Terminology
Theorem: Statement that can be shown true

Proof: Valid argument establishing truth of theorem

Axiom: Statement assumed true

Lemma: Helper theorem

Corollary: Theorem that follows directly from another

Conjecture: Statement proposed to be true (unproven)

Proof Methods
Direct proof: Assume p is true, show q must be true

Proof by contraposition: Assume ¬q is true, show ¬p is true

Proof by contradiction: Assume p is false (¬p true), derive contradiction

Proof by cases: Consider all possible cases

Existence proofs:

Constructive: Find element with desired property

Nonconstructive: Prove existence without finding element

Definitions
Even integer: n = 2k for some integer k

Odd integer: n = 2k + 1 for some integer k

Rational number: r = p/q where p, q integers, q ≠ 0

# 1.8 Proof Methods and Strategy
Exhaustive Proof
Prove by checking a finite number of cases

Without Loss of Generality (WLOG)
Assume something that doesn't lose generality of proof

Common Errors
Circular reasoning (begging the question): Assuming what you're trying to prove

Incorrect use of cases: Not covering all cases


#Chapter 2: Basic Structures - Sets, Functions, Sequences, Sums, and Matrices
# 2.1 Sets
Definitions
Set: Unordered collection of distinct objects

Element/member: Object in a set, denoted a ∈ A

Roster method: List elements in braces {a, b, c}

Set builder notation: {x | property P(x)}

Important Sets
N = {0, 1, 2, 3, ...} (natural numbers)

Z = {..., -2, -1, 0, 1, 2, ...} (integers)

Z⁺ = {1, 2, 3, ...} (positive integers)

Q = {p/q | p ∈ Z, q ∈ Z, q ≠ 0} (rational numbers)

R (real numbers), C (complex numbers)

Set Equality
A = B if and only if they have the same elements

∀x(x ∈ A ↔ x ∈ B)

Subsets
A ⊆ B if every element of A is also in B

A ⊂ B (proper subset) if A ⊆ B and A ≠ B

Empty set ∅ is a subset of every set

Cardinality
|S| = number of elements in finite set S

Power Set
P(S) = set of all subsets of S

If |S| = n, then |P(S)| = 2ⁿ

Cartesian Product
A × B = {(a, b) | a ∈ A, b ∈ B}

Aⁿ = {(a₁, a₂, ..., aₙ) | aᵢ ∈ A}

# 2.2 Set Operations
Basic Operations
Operation	Notation	Definition

Union	A ∪ B	{x	x ∈ A ∨ x ∈ B}

Intersection	A ∩ B	{x	x ∈ A ∧ x ∈ B}

Difference	A - B	{x	x ∈ A ∧ x ∉ B}

Complement	Ā	{x ∈ U	x ∉ A}

Set Identities
Law	Formula

Identity	A ∪ ∅ = A, A ∩ U = A

Domination	A ∪ U = U, A ∩ ∅ = ∅

Idempotent	A ∪ A = A, A ∩ A = A

Complementation	(Ā) = A

Commutative	A ∪ B = B ∪ A, A ∩ B = B ∩ A

Associative	A ∪ (B ∪ C) = (A ∪ B) ∪ C, A ∩ (B ∩ C) = (A ∩ B) ∩ C

Distributive	A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C), A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)

De Morgan's	A ∪ B = Ā ∩ B̄, A ∩ B = Ā ∪ B̄

Absorption	A ∪ (A ∩ B) = A, A ∩ (A ∪ B) = A

Complement	A ∪ Ā = U, A ∩ Ā = ∅

Computer Representation
Bit string representation: 1 if element in set, 0 otherwise

Union = bitwise OR, Intersection = bitwise AND

# 2.3 Functions
Definition
f: A → B assigns exactly one element of B to each element of A

Domain: A, Codomain: B

f(a) = b means b is image of a, a is preimage of b

Range: Set of all images of elements of A

Types of Functions
Type	Property

One-to-one (injective)	f(a) = f(b) ⇒ a = b

Onto (surjective)	∀b ∈ B, ∃a ∈ A with f(a) = b

Bijection (one-to-one correspondence)	Both injective and surjective

Inverse Functions
If f is bijection, f⁻¹ exists

f⁻¹(b) = a when f(a) = b

Composition
(f ∘ g)(a) = f(g(a))

Domain: domain of g, Range: image of range of g under f

Important Functions
Floor: ⌊x⌋ = greatest integer ≤ x

Ceiling: ⌈x⌉ = smallest integer ≥ x

Factorial: n! = 1·2·3·...·n, 0! = 1

# 2.4 Sequences and Summations
Sequences
Function from subset of integers to a set S

aₙ denotes term for integer n

Types of Sequences
Geometric progression: a, ar, ar², ar³, ...

Arithmetic progression: a, a + d, a + 2d, a + 3d, ...

Recurrence Relations
Expresses aₙ in terms of previous terms

Example: Fibonacci sequence f₀ = 0, f₁ = 1, fₙ = fₙ₋₁ + fₙ₋₂

Summations
Sum	Closed Form

∑_{k=0}^{n} ar^k	a(r^{n+1} - 1)/(r - 1) (r ≠ 1)

∑_{k=1}^{n} k	n(n+1)/2

∑_{k=1}^{n} k²	n(n+1)(2n+1)/6

∑_{k=1}^{n} k³	[n(n+1)/2]²

∑_{k=0}^{∞} x^k	1/(1 - x) for	x	< 1

# 2.5 Cardinality of Sets
Definitions
Sets A and B have same cardinality if there's a bijection between them

|A| ≤ |B| if ∃ one-to-one function from A to B

Countable set: Finite or has same cardinality as positive integers (ℵ₀)

Uncountable set: Not countable

Important Results
Set of rational numbers Q is countable

Set of real numbers R is uncountable (Cantor diagonalization argument)

|P(S)| > |S| for any set S (Cantor's theorem)

Continuum Hypothesis
No set A exists such that ℵ₀ < |A| < 𝔠 (where 𝔠 = |R|)

# 2.6 Matrices
Definitions
m × n matrix: Rectangular array with m rows, n columns

Square matrix: m = n

Identity matrix Iₙ: 1's on diagonal, 0's elsewhere

Transpose Aᵗ: Interchange rows and columns

Symmetric matrix: A = Aᵗ

Operations
Addition: A + B = [aᵢⱼ + bᵢⱼ] (same size)

Multiplication: AB defined if A(m×k) and B(k×n)

(AB)ᵢⱼ = ∑{q=1}^{k} aᵢq b{qⱼ}

Zero-One Matrices
Entries are 0 or 1

Join A ∨ B: [aᵢⱼ ∨ bᵢⱼ] (OR)

Meet A ∧ B: [aᵢⱼ ∧ bᵢⱼ] (AND)

Boolean product A ⊙ B: cᵢⱼ = ∨{q=1}^{k} (aᵢq ∧ b{qⱼ})

# Chapter 4: Number Theory and Cryptography
# 4.1 Divisibility and Modular Arithmetic
Divisibility
a | b means a divides b (∃c such that b = ac)

Properties:

If a|b and a|c, then a|(b + c)

If a|b, then a|bc for all integers c

If a|b and b|c, then a|c

Division Algorithm
For integer a and positive integer d: ∃ unique q, r with 0 ≤ r < d

a = dq + r

quotient q = a div d

remainder r = a mod d

Congruences
a ≡ b (mod m) means m | (a - b)

Equivalent to a mod m = b mod m

Properties:

a ≡ b (mod m) and c ≡ d (mod m) ⇒ a + c ≡ b + d (mod m)

a ≡ b (mod m) and c ≡ d (mod m) ⇒ ac ≡ bd (mod m)

Arithmetic Modulo m
Zₘ = {0, 1, 2, ..., m-1}

a +ₘ b = (a + b) mod m

a ·ₘ b = (a · b) mod m

# 4.2 Integer Representations and Algorithms
Base b Expansion
n = aₖbᵏ + aₖ₋₁bᵏ⁻¹ + ... + a₁b + a₀

Denoted (aₖaₖ₋₁...a₁a₀)ₐ

Common Bases
Binary (base 2): digits 0, 1

Octal (base 8): digits 0-7

Hexadecimal (base 16): digits 0-9, A-F (A=10, B=11, C=12, D=13, E=14, F=15)

Conversions
Binary ↔ Octal: Group binary in 3-bit blocks

Binary ↔ Hexadecimal: Group binary in 4-bit blocks

Algorithms
Addition: O(n) bit operations

Multiplication: O(n²) bit operations

Modular exponentiation: O((log m)² log n) bit operations

# 4.3 Primes and Greatest Common Divisors
Primes
Prime: Integer > 1 with only positive factors 1 and itself

Composite: Integer > 1 that's not prime

Fundamental Theorem of Arithmetic
Every integer > 1 can be written uniquely as product of primes in nondecreasing order

Trial Division
If n is composite, it has prime divisor ≤ √n

Test divisibility by all primes ≤ √n

Infinitude of Primes
There are infinitely many primes (Euclid's proof)

Distribution of Primes
Prime Number Theorem: π(x) ≈ x/ln x (where π(x) = #primes ≤ x)

Greatest Common Divisor
gcd(a, b): Largest integer dividing both a and b

Relatively prime: gcd(a, b) = 1

Pairwise relatively prime: gcd(aᵢ, aⱼ) = 1 for i ≠ j

Euclidean Algorithm
text
procedure gcd(a, b: positive integers)
x := a
y := b
while y ≠ 0
    r := x mod y
    x := y
    y := r
return x
Least Common Multiple
lcm(a, b) = ab / gcd(a, b)

# 4.4 Solving Congruences
Linear Congruences
ax ≡ b (mod m)

Solvable iff gcd(a, m) | b

Chinese Remainder Theorem
System: x ≡ a₁ (mod m₁), x ≡ a₂ (mod m₂), ..., x ≡ aₖ (mod mₖ)

If mᵢ pairwise relatively prime, solution exists and is unique modulo M = m₁m₂...mₖ

Fermat's Little Theorem
If p is prime and a not divisible by p, then a^{p-1} ≡ 1 (mod p)

For any integer a, a^p ≡ a (mod p)

Euler's Theorem
a^{φ(n)} ≡ 1 (mod n) where gcd(a, n) = 1

φ(n) = Euler's totient function = number of positive integers ≤ n relatively prime to n

# 4.5 Applications of Congruences
Hashing Functions
h(k) = k mod m assigns memory location

Pseudorandom Numbers
Linear congruential generator: x_{n+1} = (ax_n + c) mod m

Check Digits
ISBN-13: weighted sum mod 10

Credit cards: Luhn algorithm


# Chapter 6: Counting
# 6.1 The Basics of Counting
Product Rule
If procedure has m ways to do task 1 and n ways to do task 2, then there are m·n ways to do both tasks

|A × B| = |A| · |B|

Sum Rule
If task can be done in m ways or n ways (disjoint), then total = m + n

|A ∪ B| = |A| + |B| for disjoint sets

Subtraction Rule (Inclusion-Exclusion)
|A ∪ B| = |A| + |B| - |A ∩ B|

Division Rule
If task can be done in n ways, but each way counted d times, then distinct ways = n/d

# 6.2 The Pigeonhole Principle
Basic Principle
If k + 1 objects placed into k boxes, some box contains at least 2 objects

Generalized Pigeonhole Principle
If N objects placed into k boxes, some box contains at least ⌈N/k⌉ objects

# 6.3 Permutations and Combinations
Permutations (Order matters)
P(n, r) = n!/(n-r)! = number of r-permutations of n distinct elements

Combinations (Order doesn't matter)
C(n, r) = n!/(r!(n-r)!) = number of r-combinations of n distinct elements

Also denoted (ⁿᵣ) (binomial coefficient)

Important Identities
C(n, r) = C(n, n-r)

C(n, 0) = C(n, n) = 1

Pascal's identity: C(n, r) = C(n-1, r-1) + C(n-1, r)

# 6.4 Binomial Coefficients and Identities
Binomial Theorem
(x + y)ⁿ = ∑_{k=0}^{n} C(n, k) x^{n-k} y^k

Important Identities
∑_{k=0}^{n} C(n, k) = 2ⁿ

∑_{k=0}^{n} (-1)ᵏ C(n, k) = 0

∑_{k=0}^{n} k·C(n, k) = n·2ⁿ⁻¹

∑_{k=0}^{n} k²·C(n, k) = n(n+1)·2ⁿ⁻²

# 6.5 Generalized Permutations and Combinations
Permutations with Repetition
Number of r-permutations of n objects with repetition allowed: nʳ

Combinations with Repetition
Number of r-combinations from n objects with repetition allowed: C(n + r - 1, r)

Distributing Objects
Distinguishable objects into distinguishable boxes: n!/(n₁!·n₂!·...·nₖ!)

Indistinguishable objects into distinguishable boxes: C(n + k - 1, n)

Distinguishable objects into indistinguishable boxes: Stirling numbers S(n, j)

# 6.6 Generating Permutations and Combinations
Lexicographic Order
Dictionary order for permutations

Next Permutation Algorithm
Find largest j with aⱼ < aⱼ₊₁

Find smallest aₖ > aⱼ for k > j

Swap aⱼ and aₖ

Reverse sequence after position j

Next r-Combination
Given {a₁, a₂, ..., aᵣ} in increasing order

Find last aᵢ with aᵢ < n - r + i

Replace aᵢ with aᵢ + 1, then set aᵢ₊₁ = aᵢ + 1, aᵢ₊₂ = aᵢ + 2, ...

# Chapter 10: Graphs
# 10.1 Graphs and Graph Models
Definitions
Graph G = (V, E) where V = vertices, E = edges

Simple graph: No multiple edges, no loops

Multigraph: Multiple edges allowed, no loops

Pseudograph: Multiple edges and loops allowed

Directed graph (digraph): Edges have direction

Graph Models
Social networks (vertices = people, edges = friendships)

Communication networks (vertices = computers, edges = connections)

Transportation networks (vertices = cities, edges = routes)

# 10.2 Graph Terminology and Special Types
Basic Terminology
Adjacent: Vertices connected by edge

Neighbor: Vertex adjacent to given vertex

Degree deg(v): Number of edges incident to v (loops count 2)

Handshaking Theorem: ∑ deg(v) = 2|E|

# Special Graphs
Graph	Notation	Properties

Complete graph	Kₙ	Every pair of vertices adjacent

Cycle	Cₙ	n vertices in cycle (n ≥ 3)

Wheel	Wₙ	Cₙ with extra vertex connected to all

n-Cube	Qₙ	Vertices = bit strings length n

Bipartite		V = V₁ ∪ V₂, edges only between V₁ and V₂

Complete bipartite	K_{m,n}	All possible edges between parts

Subgraphs
Subgraph: Graph whose vertices and edges are subsets of original

Induced subgraph: Includes all edges between selected vertices

# 10.3 Representing Graphs and Graph Isomorphism
Representations
Adjacency list: List neighbors of each vertex

Adjacency matrix: A[i][j] = 1 if edge (i, j) exists

Incidence matrix: M[v][e] = 1 if vertex v incident to edge e

Graph Isomorphism
Graphs G₁ and G₂ isomorphic if bijection f: V₁ → V₂ preserving adjacency

f(u)f(v) ∈ E₂ iff uv ∈ E₁

Invariants: number of vertices, edges, degree sequence

# 10.4 Connectivity
Paths and Circuits
Path: Sequence of vertices with consecutive edges

Simple path: No repeated vertices

Circuit/cycle: Path with v₀ = vₙ and n ≥ 3

Connected graph: Path between every pair of vertices

Connected Components
Connected components: Maximal connected subgraphs

Connectivity in Directed Graphs
Strongly connected: Directed path from a to b and b to a for all a, b

Weakly connected: Underlying undirected graph is connected

Vertex and Edge Connectivity
Cut vertex: Removal disconnects graph

Cut edge: Removal disconnects graph

Vertex connectivity: Minimum vertices whose removal disconnects

Edge connectivity: Minimum edges whose removal disconnects

# 10.5 Euler and Hamilton Paths
Euler Paths and Circuits
Euler circuit: Uses every edge exactly once, returns to start

Euler path: Uses every edge exactly once

Theorem: Connected graph has Euler circuit iff all vertices have even degree

Theorem: Connected graph has Euler path iff exactly 0 or 2 vertices have odd degree

Hamilton Paths and Circuits
Hamilton circuit: Visits each vertex exactly once, returns to start

Hamilton path: Visits each vertex exactly once

Dirac's theorem: If deg(v) ≥ n/2 for all v in graph with n ≥ 3, then graph has Hamilton circuit

Ore's theorem: If deg(u) + deg(v) ≥ n for all nonadjacent u, v, then graph has Hamilton circuit

# 10.6 Shortest-Path Problems
Dijkstra's Algorithm
Finds shortest path from a to all vertices in weighted graph with nonnegative weights

text
procedure Dijkstra(G: weighted graph with positive weights)
for each vertex v:
    dist[v] := ∞
    previous[v] := undefined
dist[start] := 0
Q := set of all vertices

while Q not empty:
    u := vertex in Q with minimum dist
    remove u from Q
    for each neighbor v of u:
        alt := dist[u] + weight(u, v)
        if alt < dist[v]:
            dist[v] := alt
            previous[v] := u
return dist[], previous[]

# 10.7 Planar Graphs
Definition
Graph that can be drawn in plane with no edge crossings

Euler's Formula
For connected planar graph: v - e + f = 2

v = vertices, e = edges, f = faces

Kuratowski's Theorem
Graph is nonplanar iff it contains subgraph homeomorphic to K₅ or K_{3,3}

# 10.8 Graph Coloring
Definitions
Proper coloring: Adjacent vertices have different colors

Chromatic number χ(G): Minimum colors needed

Properties
χ(Kₙ) = n

χ(Cₙ) = 2 if n even, 3 if n odd

Four Color Theorem: Every planar graph has χ ≤ 4

Applications
Scheduling (conflicts = edges)

Register allocation in compilers


# Chapter 11: Trees
# 11.1 Introduction to Trees
Definitions
Tree: Connected undirected graph with no simple circuits

Forest: Graph with no simple circuits (disjoint union of trees)

Rooted tree: Tree with designated root

Parent/child: Adjacent vertices with parent closer to root

Leaf: Vertex with no children

Internal vertex: Vertex with children

Properties
Tree with n vertices has n - 1 edges

Unique simple path between any two vertices

Adding one edge creates exactly one simple circuit

m-ary Trees
m-ary tree: Every internal vertex has ≤ m children

Full m-ary tree: Every internal vertex has exactly m children

Binary tree: m = 2

Theorems
Full m-ary tree with i internal vertices has n = mi + 1 vertices

Full m-ary tree with n vertices has i = (n - 1)/m internal vertices

Height h of m-ary tree: leaves ≤ mʰ, internal vertices ≤ (mʰ - 1)/(m - 1)

# 11.2 Applications of Trees
Binary Search Trees
For each vertex: left subtree has smaller values, right subtree has larger values

Operations: search, insert, delete

Decision Trees
Each internal node = decision, leaves = outcomes

Sorting lower bound: Ω(n log n) comparisons

Prefix Codes
Variable-length codes with no codeword as prefix of another

Huffman coding: Optimal prefix code

Game Trees
Vertices = game states, edges = moves

Minimax algorithm for two-player games

# 11.3 Tree Traversal
Traversal Orders
Order	Process order

Preorder	Root, left subtree, right subtree

Inorder	Left subtree, root, right subtree

Postorder	Left subtree, right subtree, root

Infix, Prefix, Postfix Notation

Infix: Operand operator operand (needs parentheses)

Prefix (Polish): Operator operand operand

Postfix (Reverse Polish): Operand operand operator

# 11.4 Spanning Trees
Definitions
Spanning tree: Subgraph that is tree containing all vertices

Every connected graph has spanning tree

Algorithms
Depth-First Search (DFS)

```text
procedure DFS(G: graph)
T := empty graph
for each vertex v:
    mark v unvisited
for each unvisited vertex v:
    DFS-visit(v)

procedure DFS-visit(v)
mark v visited
for each neighbor w of v:
    if w unvisited:
        add edge vw to T
        DFS-visit(w)
Breadth-First Search (BFS)
```
```text
procedure BFS(G: graph)
T := empty graph
for each vertex v:
    mark v unvisited
for each unvisited vertex v:
    BFS-visit(v)

procedure BFS-visit(v)
initialize empty queue Q
mark v visited
enqueue v to Q
while Q not empty:
    dequeue v from Q
    for each neighbor w of v:
        if w unvisited:
            mark w visited
            add edge vw to T
            enqueue w to Q
```

# 11.5 Minimum Spanning Trees
Definition
Weighted graph: Find spanning tree with minimum total weight

Prim's Algorithm
Grows tree from starting vertex

```text
procedure Prim(G: weighted connected graph)
T := empty set
V_T := {v₀} (arbitrary starting vertex)

while V_T ≠ V:
    choose edge (u, v) with minimum weight
    where u ∈ V_T, v ∉ V_T
    add v to V_T
    add edge (u, v) to T
return T
Kruskal's Algorithm
Adds edges in increasing weight order, avoiding cycles
```
```text
procedure Kruskal(G: weighted connected graph)
T := empty set
sort edges by increasing weight
for each edge (u, v) in sorted order:
    if u and v are in different components of T:
        add edge (u, v) to T
return T
```
