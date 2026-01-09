
# Groups


degree n
order n!


---

List all subgroups of $S_5$ up to isomorphism.

| Group | Degree | Order | Composition Series                                        | Composition Factors                                         | Simple | Abelian |
| ----- | ------ | ----- | --------------------------------------------------------- | ----------------------------------------------------------- | ------ | ------- |
| S₁    | 1      | 1     | $1$                                                       | –                                                           | -      | Yes     |
| S₂    | 2      | 2     | $1 \triangleleft S_2$                                     | $\mathbb{Z}_2$                                              | Yes    | Yes     |
| C₃    | 3      | 3     | $1 \triangleleft C_3$                                     | $\mathbb{Z}_3$                                              | Yes    | Yes     |
| S₃    | 3      | 6     | $1 \triangleleft A_3 \triangleleft S_3$                   | $\mathbb{Z}_3,\ \mathbb{Z}_2$                               | -      | -       |
| C₄    | 4      | 4     | $1 \triangleleft C_2 \triangleleft C_4$                   | $\mathbb{Z}_2,\ \mathbb{Z}_2$                               | -      | Yes     |
| V₄    | 4      | 4     | $1 \triangleleft V_4$                                     | $\mathbb{Z}_2,\ \mathbb{Z}_2$                               | -      | Yes     |
| D₄    | 4      | 8     | $1 \triangleleft C_2 \triangleleft V_4 \triangleleft D_4$ | $\mathbb{Z}_2,\ \mathbb{Z}_2,\ \mathbb{Z}_2$                | -      | -       |
| A₄    | 4      | 12    | $1 \triangleleft V_4 \triangleleft A_4$                   | $\mathbb{Z}_3,\ \mathbb{Z}_2,\ \mathbb{Z}_2$                | -      | -       |
| S₄    | 4      | 24    | $1 \triangleleft A_4 \triangleleft S_4$                   | $\mathbb{Z}_3,\ \mathbb{Z}_2,\ \mathbb{Z}_2,\ \mathbb{Z}_2$ | -      | -       |
| C₅    | 5      | 5     | $1 \triangleleft C_5$                                     | $\mathbb{Z}_5$                                              | Yes    | Yes     |
| D₅    | 5      | 10    | $1 \triangleleft C_5 \triangleleft D_5$                   | $\mathbb{Z}_5,\ \mathbb{Z}_2$                               | -      | -       |
| A₅    | 5      | 60    | $1 \triangleleft A_5$                                     | $A_5$                                                       | Yes    | -       |
| S₅    | 5      | 120   | $1 \triangleleft A_5 \triangleleft S_5$                   | $A_5,\ \mathbb{Z}_2$                                        | -      | -       |

- **V₄** (Klein four-group) is **not simple** and **has no composition series** with simple (non-abelian) factors unless split further trivially (but all its subgroups are of order 2 and not normal chains).
* Abelian = commutative


---

Degree 1

Symmetric group $S_1$ (1)


Degree 2

Symmetric group $S_2$ (2)


Degree 3

Cyclic group $C_3$ (3)
Symmetric group $S_3$ (6)


Degree 4

Cyclic group $C_4$ (4)
Klein four-group $V_4$ (4)
Dihedral group $D_4$ (8)
Alternating group $A_4$ (12)
Symmetric group $S_4$ (24)


---

## Lagrange's Theorem

Lagrange's Theorem states that for any finite group G, the order (number of elements) of every subgroup H must divide the order of the group G.


---

## Jordan-Hölder

The Jordan-Hölder theorem tells us that while a group can have multiple composition series, the set of **composition factors** (the simple groups that appear as quotients in the series) is unique up to isomorphism and order.


---

## Composition Series


In group theory, a **composition series** provides a way to break down a group into its "simple pieces," analogous to how integers can be factored into prime numbers.

More formally, a **composition series** of a group G is a finite sequence of subgroups:

$G = G_0 ​⊃ G_1 ​⊃ G_2 ​⊃ ⋯ ⊃ G_n ​= \{e\}$

where:

1. All inclusions are strict (i.e., Gi​=Gi+1​).
2. Each Gi+1​ is a normal subgroup of Gi​ (denoted Gi+1​◃Gi​). This type of sequence is called a **subnormal series**.
3. Each **factor group** (or quotient group) Gi​/Gi+1​ is a **simple group**. A simple group is a non-trivial group whose only normal subgroups are the trivial subgroup and the group itself. These factor groups are called **composition factors**.


---

## Lie Groups

...

