
To derive the eigenstates of the total spin for three spin-$1/2$ particles, we use the addition of angular momentum. For a single particle, the spin is $s = 1/2$. When we combine three such particles, the total Hilbert space has a dimension of $2^3 = 8$.

We decompose the total spin $S$ by adding the particles one by one:

1. **Combine first two spins:** $1/2 \otimes 1/2 = 1 \oplus 0$.
    
2. **Add the third spin:** $(1 \oplus 0) \otimes 1/2 = (1 \otimes 1/2) \oplus (0 \otimes 1/2)$.
    
3. **Result:** $3/2 \oplus 1/2 \oplus 1/2$.
    

This results in one **quadruplet** ($S=3/2$) and two **doublets** ($S=1/2$).

---

## 1. The Quadruplet States ($S = 3/2$)

These states are fully symmetric under the exchange of any two particles. We start with the "stretched" state (maximum $M_S$) and apply the lowering operator $S_- = s_{1-} + s_{2-} + s_{3-}$.

- **$|3/2, 3/2\rangle$**:
    $$|3/2, 3/2\rangle = |+++\rangle$$
    
- **$|3/2, 1/2\rangle$** (Apply $S_-$ to the above and normalize):
    $$|3/2, 1/2\rangle = \frac{1}{\sqrt{3}} \left( |++-\rangle + |+-+\rangle + |-++\rangle \right)$$
    
- **$|3/2, -1/2\rangle$**:
    $$|3/2, -1/2\rangle = \frac{1}{\sqrt{3}} \left( |--+\rangle + |-+-\rangle + |+--\rangle \right)$$
    
- **$|3/2, -3/2\rangle$**:
    $$|3/2, -3/2\rangle = |---\rangle$$
    

---

## 2. The First Doublet ($S = 1/2$)

We derive these by coupling the first two particles to a **triplet** state ($S_{12} = 1$) and then adding the third particle to reach a total $S = 1/2$. Using Clebsch-Gordan coefficients for $1 \otimes 1/2 \to 1/2$:

- **$|1/2, 1/2\rangle_1$**:
    $$|1/2, 1/2\rangle_1 = \sqrt{\frac{2}{3}} |S_{12}=1, M_{12}=1\rangle |-\rangle - \sqrt{\frac{1}{3}} |S_{12}=1, M_{12}=0\rangle |+\rangle$$
    
    Expanding the $S_{12}$ states:
    
    $$|1/2, 1/2\rangle_1 = \frac{1}{\sqrt{6}} \left( 2|++-\rangle - |+-+\rangle - |-++\rangle \right)$$
    
- **$|1/2, -1/2\rangle_1$** (By symmetry or $S_-$):
    $$|1/2, -1/2\rangle_1 = \frac{1}{\sqrt{6}} \left( |+--\rangle + |-+-\rangle - 2|--+\rangle \right)$$
    

---

## 3. The Second Doublet ($S = 1/2$)

This pair arises from coupling the first two particles to a **singlet** state ($S_{12} = 0$). Adding the third particle is straightforward because $0 \otimes 1/2$ can only result in $1/2$.

- **$|1/2, 1/2\rangle_2$**:
    $$|1/2, 1/2\rangle_2 = |S_{12}=0, M_{12}=0\rangle |+\rangle$$
    
    Expanding the singlet $|S_{12}=0\rangle = \frac{1}{\sqrt{2}}(|+-\rangle - |-+ \rangle)$:
    
    $$|1/2, 1/2\rangle_2 = \frac{1}{\sqrt{2}} \left( |+-+\rangle - |-++\rangle \right)$$
    
- **$|1/2, -1/2\rangle_2$**:
    $$|1/2, -1/2\rangle_2 = \frac{1}{\sqrt{2}} \left( |+--\rangle - |-+-\rangle \right)$$
    

---

### Summary of States

The 8 basis states are organized by their total spin quantum numbers $|S, M_S\rangle$:

| **Total S**      | **MS​** | **State Expression**   |
| ---------------- | ------- | ---------------------- |
| **3/2**          | +3/2    | $\|3/2, 3/2\rangle$    |
|                  | +1/2    | $\|3/2, 1/2\rangle$    |
|                  | -1/2    | $\|3/2, -1/2\rangle$   |
|                  | -3/2    | $\|3/2, -3/2\rangle$   |
| **1/2 (Type 1)** | +1/2    | $\|1/2, 1/2\rangle_1$  |
|                  | -1/2    | $\|1/2, -1/2\rangle_1$ |
| **1/2 (Type 2)** | +1/2    | $\|1/2, 1/2\rangle_2$  |
|                  | -1/2    | $\|1/2, -1/2\rangle_2$ |

Are you looking to apply these to a specific Hamiltonian, like the Heisenberg exchange model, or was the derivation itself the main goal?