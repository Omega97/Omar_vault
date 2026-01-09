

In quantum computing, let's imagine a computation where we start the computation in a state $\ket{\psi_0}=\sum_{n}{c_n \ket{n}}$, and apply a quantum circuit $U$. In this case, $U \ket{\psi_0}=\sum_{n}{c_n U \ket{n}}$, which suggests that you can take independently each classical state, and see where the quantum gate takes it, to then recombine all the results at the end based on the initial state $\ket{\psi_0}$. 

The modulus squared of the $c_n$ coefficients can be interpreted as the probability $p_n=|c_n|^2$ of getting the $\ket{n}$ state when measuring $\ket{\psi}$. In a way, the observer is in a superposition, identical in all the "Many World" strands, and, at the time of measurement, they get entangled with the observed system, and the various strands "diverge", or, more properly, become distinct.

---

#### Example 1 - an observer 👀, and states 🔴🔵


We start from the state:
$$\frac{1}{\sqrt2}(\ket{🔴} + \ket{🔵}) \otimes \ket{👀} =  \frac{1}{\sqrt2} (\ket{🔴,👀} + \ket{🔵,👀})$$
after observation, it becomes:
$$\frac{1}{\sqrt2} (\ket{🔴,👀} + \ket{🔵,👀}) \rightarrow \frac{1}{\sqrt2} (\ket{🔴,🔴👀} + \ket{🔵,🔵👀})$$
But of course, the observer doesn't see the strands where he is in a different quantum state (for example, he observed a different outcome). Let's make an example with an observer 👀 that can count the 🔵.

---

#### Example 2 - counting the 🔵


We start in the state:
$$(H^{\otimes2} \ket{🔴🔴}) \otimes \ket{👀} = \frac{1}{2} (\ket{🔴🔴} + \ket{🔴🔵} + \ket{🔵🔴} + \ket{🔵🔵}) \otimes \ket{👀}$$
After observing the number of $🔵$ we get:
$$\frac{1}{2} (\ket{🔴🔴,0🔵👀} + \ket{🔴🔵,1🔵👀} + \ket{🔵🔴,1🔵👀} + \ket{🔵🔵,2🔵👀})$$
The observer that measured 1🔵 is in a superposition, so we group the like observers to get:
$$\frac{1}{2}\ket{🔴🔴,0🔵👀} + \frac{1}{2}(\ket{🔴🔵} + \ket{🔵🔴}) \otimes \ket{1🔵👀} + \frac{1}{2}\ket{🔵🔵,2🔵👀}$$
The world "branched" in 3, with 25%, 50%, and 25% probability respectively.

---

#### Example 3 - recombining the strands


For this example, we assume that the observer is just a quantum system that can remember a measurement.
The 4 classical states are:
- $\ket{🔴,👀}$
- $\ket{🔴,🔴👀}$
- $\ket{🔵,👀}$
- $\ket{🔵,🔵👀}$

We start with a qubit in the state 🔴.
$$\ket{\psi_1} = \ket{🔴,👀}$$
Then, we apply the *Hadamard* operator to split the branches;
$$\ket{\psi_2} = H \ket{🔴} \otimes \ket{👀} = \frac{1}{\sqrt2} (\ket{🔴,👀} + \ket{🔵,👀})$$
Next, the observer performs the measurement.
$$\ket{\psi_3} = \frac{1}{\sqrt2} (\ket{🔴,🔴👀} + \ket{🔵,🔵👀})$$
From their point of view, the observer $\ket{🔴👀}$ is in the exact same state as id they immediately performed a measurement in $\ket{\psi_1}$. 


---
The 4 classical states are:
- $\ket{🔴,👀}$
- $\ket{🔴,🔴👀}$
- $\ket{🔵,👀}$
- $\ket{🔵,🔵👀}$

In this same basis, the measurement operator can be thought of as 
$$\begin{bmatrix}
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0
\end{bmatrix}$$
So $U_{measure}=I \otimes X$
Is this correct?

---

My question is a bit of a vague one. 

> "What *glues* the strands together?"

I mean, if everything is linear, and the strands are therefore independent, why is the case that we live in a quantum universe? What's the mechanism that governs the 
