


---

## 1. Foundational Geometric Structures


#### Admitting

Allowing a structure (e.g., a [[Differential Geometry 🔹#Metric Tensor|metric]] or [[Differential Geometry 🔹#Gauge connections|connection]]) to exist compatibly on a [[Differential Geometry 🔹#Manifold|manifold]] or space, crucial for defining consistent geometric or physical properties.

#### Affine Spaces

Vector spaces without a fixed origin, allowing translations but no absolute reference point. Points are defined relative to each other via vector differences. [[Differential Geometry 🔹#Vector bundles|Vector bundles]] often generalize this idea.

#### Choosing a signature
Selecting the signature of a [[Differential Geometry 🔹#Metric Tensor|metric tensor]] (e.g., (+,−,−,−) for Minkowski spacetime), determining the geometry of a [[Differential Geometry 🔹#Manifold|manifold]].

#### Manifold

A topological space that locally resembles Euclidean space, enabling calculus in curved settings, such as spacetime in [[Differential Geometry 🔹#Einstein tensor|general relativity]] or [[Differential Geometry 🔹#Calabi–Yau manifold|Calabi–Yau manifolds]].

---

#### Metric Tensor

A tensor defining distances, angles, and geometry on a [[Differential Geometry 🔹#Manifold|manifold]]. It underpins [[Differential Geometry 🔹#Riemannian curvature tensors|Riemannian geometry]] and [[Differential Geometry 🔹#Einstein’s field equations|Einstein’s field equations]].

#### Space of metrics

The set of all possible [[Differential Geometry 🔹#Metric Tensor|metric tensors]] on a [[Differential Geometry 🔹#Manifold|manifold]], used to study geometric variations, as in [[Differential Geometry 🔹#Einstein tensor|general relativity]].

## 2. Fiber Bundles & Topology


#### Associated bundle

A [[Differential Geometry 🔹#Fiber bundles|fiber bundle]] constructed from a [[Differential Geometry 🔹#Principal bundle|principal bundle]] by attaching a fiber (e.g., a vector space) via a group action, used in [[Differential Geometry 🔹#Gauge theory|gauge theories]].

#### Chern class

A topological invariant of a [[Differential Geometry 🔹#Vector bundles|vector bundle]], measuring its “twisting,” used in [[Differential Geometry 🔹#Calabi–Yau manifold|complex geometry]] and gauge theories.

---

#### Fiber bundles

Spaces that locally resemble a product of a base space and a fiber (e.g., a vector space), used to model structures like [[Differential Geometry 🔹#Vector bundles|vector bundles]] or [[Differential Geometry 🔹#Principal bundle|principal bundles]] in physics and geometry.

#### Fibration

A continuous map from a total space to a base space, where each point in the base has a fiber (a consistent structure, like a circle or vector space) attached, preserving local geometry.

#### Fundamental Groups

Topological invariants that capture the structure of loops in a space, describing its “holes” in one dimension. They help classify spaces like [[Differential Geometry 🔹#Manifold|manifolds]].

#### Gauge connections

Fields in a [[Differential Geometry 🔹#Fiber bundles|fiber bundle]] defining parallel transport, central to [[Differential Geometry 🔹#Gauge theory|gauge theories]] like electromagnetism or [[Differential Geometry 🔹#Yang-Mills theory|Yang-Mills]].

#### Homology Groups

Algebraic invariants measuring “holes” in a topological space at various dimensions, complementing [[Differential Geometry 🔹#Fundamental Groups|fundamental groups]] in classifying spaces.

#### Principal bundle

A [[Differential Geometry 🔹#Fiber bundles|fiber bundle]] with a [[Differential Geometry 🔹#Lie Group|Lie group]] as its fiber, acted upon freely by the group, foundational in [[Differential Geometry 🔹#Gauge theory|gauge theories]].

#### Tangent bundle

A [[Differential Geometry 🔹#Vector bundles|vector bundle]] where the fiber at each point of a [[Differential Geometry 🔹#Manifold|manifold]] is its tangent space, used to define [[Differential Geometry 🔹#Covariant derivative|covariant derivatives]] and study differential geometry.

#### Stone duality

A mathematical bridge between topology and algebra, establishing a dual equivalence between Stone spaces (compact, totally disconnected Hausdorff spaces) and Boolean algebras.

## 3. Connections, Transport, & Derivatives


#### Affine connection

...

#### Choice of connection

Selecting a [[Differential Geometry 🔹#Gauge connections|connection]] (e.g., [[Differential Geometry 🔹#Levi-Civita connection|Levi-Civita]]) on a [[Differential Geometry 🔹#Manifold|manifold]] or [[Differential Geometry 🔹#Fiber bundles|bundle]], defining parallel transport in geometric and physical contexts.

#### Connection

A mathematical object defining [[Differential Geometry 🔹#Parallel transport|parallel transport]] of vectors or tensors on a [[Differential Geometry 🔹#Manifold|manifold]] or [[Differential Geometry 🔹#Fiber bundles|bundle]], such as in [[Differential Geometry 🔹#Gauge theory|gauge theories]].


---

#### Covariant derivative

A derivative on a [[Differential Geometry 🔹#Manifold|manifold]] that respects its geometric structure, preserving [[Differential Geometry 🔹#Metric Tensor|metrics]] or [[Differential Geometry 🔹#Gauge connections|connections]], used in [[Differential Geometry 🔹#Einstein tensor|general relativity]].

#### Holonomy

The [holonomy](https://en.wikipedia.org/wiki/Holonomy) of a **connection** on a smooth manifold is t**he extent to which parallel transport around closed loops fails to preserve the geometrical data being transported**. Holonomy is a general geometrical consequence of the curvature of the connection. For flat connections, the associated holonomy is a type of monodromy and is an inherently global notion. For curved connections, holonomy has nontrivial local and global features.

#### Levi-Civita connection

The unique torsion-free [[Differential Geometry 🔹#Gauge connections|connection]] on a [[Differential Geometry 🔹#Manifold|manifold]] preserving the [[Differential Geometry 🔹#Metric Tensor|metric]], used in [[Differential Geometry 🔹#Riemannian curvature tensors|Riemannian geometry]].

#### Parallel transport

The process of moving a geometric object (like a vector) along a curve such that it stays "constant" relative to a [[Differential Geometry 🔹#Connection|connection]].

#### Pulling back
Using a map to transfer geometric objects, like [[Differential Geometry 🔹#Differential form|forms]] or [[Differential Geometry 🔹#Metric Tensor|tensors]], from one [[Differential Geometry 🔹#Manifold|manifold]] to another, preserving structure.

## 4. Curvature & Tensor Calculus




---

#### Contraction

Summing over repeated indices of a tensor to reduce its rank, used in operations like forming the [[Differential Geometry 🔹#Ricci curvature tensor|Ricci tensor]] from the [[Differential Geometry 🔹#Riemannian curvature tensors|Riemann tensor]].

#### Differential form

A mathematical object that is antisymmetric under coordinate changes and can be integrated over [[Differential Geometry 🔹#Manifold|manifolds]]. Used to describe fields, such as electromagnetic potentials, in a coordinate-independent way.

#### Pseudo-tensor
An object transforming like a tensor under specific coordinate changes (e.g., proper Lorentz transformations), but not others, unlike true tensors in [[Differential Geometry 🔹#Einstein tensor|general relativity]].

#### Ricci curvature tensor

A tensor obtained by [[Differential Geometry 🔹#Contraction|contracting]] the [[Differential Geometry 🔹#Riemannian curvature tensors|Riemann curvature tensor]], measuring how volumes distort in a [[Differential Geometry 🔹#Manifold|manifold]]. It is critical in [[Differential Geometry 🔹#Einstein’s field equations|Einstein’s field equations]].

#### Riemannian curvature tensors

Tensors describing the intrinsic curvature of a [[Differential Geometry 🔹#Manifold|manifold]] with a [[Differential Geometry 🔹#Metric Tensor|metric]], used in [[Differential Geometry 🔹#Einstein tensor|general relativity]].

#### Structure Tensor 
A tensor encoding algebraic or geometric properties, such as torsion or curvature, in structures like [[Differential Geometry 🔹#Manifold|manifolds]] or [[Differential Geometry 🔹#Lie Group|Lie groups]].

#### Torsion tensor

A tensor measuring the failure of a [[Differential Geometry 🔹#Connection|connection]] to be symmetric, describing twisting in a [[Differential Geometry 🔹#Manifold|manifold]]’s geometry. The [[Differential Geometry 🔹#Levi-Civita connection|Levi-Civita connection]] has zero torsion.

#### Trace-reversing
Subtracting the trace of a tensor (e.g., [[Differential Geometry 🔹#Metric Tensor|metric]] or [[Differential Geometry 🔹#Einstein tensor|Einstein tensor]]) to obtain its traceless part, often used in [[Differential Geometry 🔹#Einstein tensor|general relativity]].

## 5. Gauge Theory & Quantum Physics



---

#### Gauge group

The group of local transformations (e.g., phase changes) leaving a [[Differential Geometry 🔹#Gauge theory|gauge theory]] invariant, such as U(1) in electromagnetism or SU(3) in QCD.

#### Gauge theory

A field theory where physical laws are invariant under local [[Differential Geometry 🔹#Gauge group|gauge transformations]], describing fundamental interactions like electromagnetism or [[Differential Geometry 🔹#Yang-Mills theory|Yang-Mills]].

#### Gauge transformation

A local change of reference frame in a [[Differential Geometry 🔹#Gauge theory|gauge theory]], preserving physical predictions, such as shifting the electromagnetic potential.

#### U(1)

...

#### Symmetry breaking

A process where a system’s symmetry is reduced, often spontaneously, leading to new physical phenomena. It is key in the [[Differential Geometry 🔹#Higgs Mechanism|Higgs mechanism]] and phase transitions in [[Differential Geometry 🔹#Gauge theory|gauge theories]].

#### Yang-Mills theory 

A [[Differential Geometry 🔹#Gauge theory|gauge theory]] with non-Abelian [[Differential Geometry 🔹#Gauge group|gauge groups]], describing fundamental interactions like the strong force in quantum chromodynamics.

## 6. Spinors & Algebras


#### Clifford Algebra

An algebra generated by vectors under a quadratic form (e.g., a [[Differential Geometry 🔹#Metric Tensor|metric]]), used to define [[Differential Geometry 🔹#Spinor|spinors]] and [[Differential Geometry 🔹#Dirac operator|Dirac operators]] in quantum field theory.

#### Dirac operator

A differential operator acting on [[Differential Geometry 🔹#Spinor|spinor fields]], crucial in quantum field theory for describing fermion dynamics, such as electrons in relativistic settings.

---

#### Double cover

A topological construction where a covering space (e.g., [[Differential Geometry 🔹#Spin(X,Y)|Spin(X,Y)]]) maps two points to one in the base space (e.g., [[Differential Geometry 🔹#SO(1,3)|SO(X,Y)]]), enabling [[Differential Geometry 🔹#Spinor|spinor representations]].

#### Frobenius Inner Product

The inner product on a [[Differential Geometry 🔹#Clifford Algebra|Clifford algebra]] or matrix algebra, often used to define norms or traces in geometric and algebraic contexts.

#### Passing to the double cover
Transitioning from a group (e.g., [[Differential Geometry 🔹#SO(1,3)|SO(1,3)]]) to its [[Differential Geometry 🔹#Double cover|double cover]] (e.g., [[Differential Geometry 🔹#Spin(X,Y)|Spin(1,3)]]) to enable [[Differential Geometry 🔹#Spinor representation|spinor representations]].

#### Spin-10

The double cover of the [[Differential Geometry 🔹#SO(10)|SO(10)]] group, denoted Spin(10), enabling [[Differential Geometry 🔹#Spinor representation|spinor representations]] in 10 dimensions; central to SO(10) GUTs for describing chiral fermions and supersymmetric extensions in string theory.


#todo Petit-Salam; SU(3) vs Spin 6; Displace (augmented) torsion tensor; Wu-Yeng; 

#### Spinor

A mathematical object transforming under [[Differential Geometry 🔹#Spin(X,Y)|spin groups]], used to describe fermions (e.g., electrons) in quantum mechanics and relativity.

#### Spinor representation

A linear action of [[Differential Geometry 🔹#Spin(X,Y)|Spin groups]] on [[Differential Geometry 🔹#Spinor|spinor fields]], crucial for describing fermions in quantum field theory.

#### Weyl spinors
Two-component [[Differential Geometry 🔹#Spinor|spinors]] describing massless fermions, transforming under the [[Differential Geometry 🔹#Spin(X,Y)|Spin group]], used in chiral theories.

## 7. Symmetry Groups & Unified Theories


#### CKM Matrix

The Cabibbo-Kobayashi-Maskawa matrix, describing quark flavor mixing in weak interactions within the Standard Model, linking quark states via [[Differential Geometry 🔹#Gauge theory|gauge symmetries]].

#### Lie Group

A group that is also a smooth [[Differential Geometry 🔹#Manifold|manifold]], where group operations (multiplication, inversion) are smooth maps. Examples include [[Differential Geometry 🔹#SO(3)|SO(3)]] and [[Differential Geometry 🔹#Lorentz Group|Lorentz Group]].

#### Lorentz Group - SO(1,3)

The group of transformations preserving the spacetime interval in special relativity, denoted [[Differential Geometry 🔹#SO(1,3)|SO(1,3)]]. It describes rotations and boosts in 4D Minkowski spacetime.
The [[Differential Geometry 🔹#Lorentz Group - SO(1,3)|Lorentz group]] in 4D Minkowski spacetime, preserving the spacetime interval. It is a [[Differential Geometry 🔹#Lie Group|Lie group]] central to special relativity.


#### $M_{PMNS}$ Matrix

The Pontecorvo-Maki-Nakagawa-Sakata matrix, describing neutrino flavor mixing in weak interactions, analogous to the [[Differential Geometry 🔹#CKM Matrix|CKM matrix]] for quarks.

#### Pati-Salam 

A grand unified theory extending the Standard Model, unifying quarks and leptons under a larger [[Differential Geometry 🔹#Gauge group|gauge group]] (e.g., SU(4)×SU(2)×SU(2)).

#### SO(3)

The [[Differential Geometry 🔹#Lie Group|Lie group]] of rotations in 3D Euclidean space, describing symmetries of physical systems like angular momentum.

#### SO(10)

A [[Differential Geometry 🔹#Lie Group|Lie group]] of 10-dimensional orthogonal transformations with positive determinant, used in grand unified theories (GUTs) to unify the Standard Model gauge groups ([[Differential Geometry 🔹#Gauge group|SU(3)×SU(2)×U(1)]]) into a single representation, accommodating quarks, leptons, and their interactions in 16-dimensional [[Differential Geometry 🔹#Spinor representation|spinor representations]].

#### Spin(X,Y)

The double cover of the [[Differential Geometry 🔹#SO(1,3)|SO(X,Y)]] group, enabling [[Differential Geometry 🔹#Spinor representation|spinor representations]] for particles with half-integer spin.


---

## 8. Complex Geometry & Specialized Terms


#### Bilinear form

A function that takes two vectors and is linear in each, like the inner product on a vector space or the [[Differential Geometry 🔹#Metric Tensor|metric tensor]] on a [[Differential Geometry 🔹#Manifold|manifold]], foundational for geometry and physics.

#### Calabi–Yau manifold

A compact, complex [[Differential Geometry 🔹#Kähler manifold|Kähler manifold]] with a vanishing first [[Differential Geometry 🔹#Chern class|Chern class]], admitting a [[Differential Geometry 🔹#Ricci curvature tensor|Ricci]]-flat [[Differential Geometry 🔹#Metric Tensor|metric]]. These manifolds are pivotal in string theory, compactifying extra dimensions (typically from 10 to 4) while preserving supersymmetry.


---

#### Chimeric bundle
A speculative or niche term, possibly referring to a [[Differential Geometry 🔹#Fiber bundles|fiber bundle]] with mixed or hybrid fiber structures, combining features like vector and principal bundles (needs context for precision).

#### Frobenius metric

A [[Differential Geometry 🔹#Metric Tensor|metric]] compatible with a Frobenius manifold, where the curvature satisfies specific algebraic conditions, often studied in topological field theory.


#### Kähler manifold

A [[Differential Geometry 🔹#Manifold|manifold]] with a compatible complex structure, symplectic structure, and [[Differential Geometry 🔹#Metric Tensor|metric]], used in [[Differential Geometry 🔹#Calabi–Yau manifold|string theory]] and complex geometry.

#### Lie Algebra Cohomology

An algebraic tool measuring invariants of a [[Differential Geometry 🔹#Lie Group|Lie group]]’s associated Lie algebra, used in symmetry analysis and [[Differential Geometry 🔹#Gauge theory|gauge theories]].

#### Observation map
A map assigning measurement outcomes to geometric or physical data, often in the context of [[Differential Geometry 🔹#Observers|observers]] or [[Differential Geometry 🔹#Gauge theory|field theories]].

#### Vector bundles

A [[Differential Geometry 🔹#Manifold|manifold]] with a vector space attached at each point, generalizing tangent spaces. Used in [[Differential Geometry 🔹#Gauge theory|gauge theories]] and [[Differential Geometry 🔹#Fiber bundles|fiber bundles]].


