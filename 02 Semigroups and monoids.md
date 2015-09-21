Semigroups and monoids
======================



A *semigroup* $S$ is a set $S \times S \to S$ with and internal operation
$(x,y) \to x \cdot y$ which is associative: for all $x,y,z \in S$, we have
$(x \cdot y) \cdot z = x \cdot (y \cdot z)$.

A *monoid* $M$ is a semigroup with a neutral element $1_M$: for all $x \in S$,
we have $x \cdot 1_M = 1_M \cdot x = x$.

Examples:

- $(\mathbb{N}, +)$
- $(\mathbb{Z}, +)$
- groups
- $A^*$ concatenation (*free*-monoid). Without the empty word, it's only a semigroup.
- Any set $E$, with $max$ is a semigroup. In order to be a monoid you need to
add a absolute maximum.
- matrices over semi-ring
- functions $E \to E$
- relations

You can always turn a semigroup $S$ into a monoid $S^1$:

- If it has already a neutral element, then it is already a monoid.
- If not, add one. And extend the multiplication table.

A *morphis* of semigroups is a function $\mu : S \to T$ with
$\forall s, s' \in S, \mu(s \cdot s') = \mu(s) \cdot \mu(s')$.

A morphism of monoids is a morphism of semigroups $\mu : S \to T$ with
$\mu(1_S) = A_T$.

Examples:

- $(A^*, \cdot) \to \mathbb{N}, + : w \mapsto |w|$ (length)
- The determinent of matrices.

Definition:
A morphism of monoids $\mu : M \to N$ recognizes $L \in M$ if there exists
$P \in N$ such that $L = \mu^{-1}(P)$.

[…]

\begin{theorem}
$L \in A^*$ is *rational* iff it is recognizable by a **finite** morphism
$\mu : A^* \to N$.
\end{theorem}

Examples:

1. $\mu : A^* \longmapsto |N| mod 2$
   $P = {0}$. $L = \mu^{-1}(0) = (AA)^*$

2. $A* \longmapsto M = {\alpha, \beta, 1}$



Division of monoids
-------------------

A sub-semigroup (resp. sub-monoid) is a semigroup contained in an other one, and
with the restriction of the product of the other one.

A quotient 
