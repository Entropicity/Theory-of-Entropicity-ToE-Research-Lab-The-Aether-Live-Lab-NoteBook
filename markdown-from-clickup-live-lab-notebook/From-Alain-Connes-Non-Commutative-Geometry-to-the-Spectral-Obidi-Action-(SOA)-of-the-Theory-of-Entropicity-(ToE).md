# From Alain Connes' Non-Commutative Geometry to the Spectral Obidi Action (SOA) of the Theory of Entropicity (ToE)—Some Critical Remarks 

# Is the Spectral Obidi Action (SOA) not a repetition of what Alain Connes and others have already done in previous research works?

From-Alain-Connes-Non-Commutative-Geometry-to-the-Spectral-Obidi-Action-(SOA)-of-the-Theory-of-Entropicity-(ToE).md

This is a sharp and fair question, and the honest answer is: **partially yes, partially no** — and the distinction matters.

## The Formal Overlap

The strategic move is the same. Connes and Chamseddine (1996) proposed:

$$S_{\text{Connes}} = \text{Tr}\, f(D/\Lambda) + \frac{1}{2}\langle J\psi, D\psi \rangle$$

where $D$ is the **Dirac operator** on a spectral triple $(A, H, D)$, $f$ is a positive even cutoff, and $\Lambda$ is a UV scale. In the low-energy asymptotic expansion via heat-kernel coefficients, this reproduces the Einstein-Hilbert action, the Standard Model Yang-Mills-Higgs terms, and a cosmological constant — all from the **spectrum of a single operator**.

Obidi's SOA:

$$S_{\text{Obidi}} = -\text{Tr}\ln(\Delta), \qquad \Delta = G[S]\, g[S]^{-1}$$

also says: "the fundamental action is a **spectral invariant** — a trace of a function of an operator — from which geometry and dynamics follow." That is the same *move*. The "derive the action from the spectrum of an operator" strategy is Connes' strategy, and Obidi is making an entropic use of it.

## Where It Is NOT a Repetition

The **ingredients** are different, and the differences are not cosmetic:

| | Connes/Chamseddine | Obidi |
|---|---|---|
| **Operator** | Dirac operator $D$ on a spectral triple | Ratio of two Laplacian-type operators $\Delta = G[S]\,g[S]^{-1}$ |
| **Function** | Arbitrary cutoff $f$ (Connes notes the choice is "largely irrelevant") | Specifically $\ln$ — the log-determinant |
| **Algebraic foundation** | Noncommutative geometry (spectral triples, $C^*$-algebras) | Information geometry (Fisher-Rao metric, $\alpha$-connections) |
| **What the spectrum encodes** | Spacetime geometry + internal gauge structure (via noncommutative algebra $A = C^\infty(M) \otimes M_4(\mathbb{C})$) | Deviation of matter-induced entropy geometry from background equilibrium |
| **Scale** | Explicit UV cutoff $\Lambda$; action is an EFT valid below $\Lambda$ | No explicit UV cutoff; structure determined by the entropic field itself |
| **Physical interpretation** | Geometry is encoded in the Dirac spectrum | Geometry is a **relative** measure: how far the entropic field is from equilibrium |

The $-\text{Tr}\ln(\Delta)$ form specifically is not the Connes form. It is the form of the **one-loop effective action** in QFT (the Gaussian path integral gives $-\frac{1}{2}\text{Tr}\ln(\Box + m^2)$) and the **zeta-function regularization** identity $\zeta_\Delta'(0) = -\text{Tr}\ln(\Delta)$. So Obidi's SOA is formally closer to the **effective action / zeta-function** tradition than to Connes' cutoff-based spectral action.

The **ratio structure** $\Delta = G[S]\,g[S]^{-1}$ — comparing two geometries — is also not in Connes. It is closer to **bimetric gravity** or **relative entropy** constructions. Connes has one Dirac operator; Obidi has a **pair** whose ratio is the fundamental object.

## The Honest Assessment

The **general strategy** — "a single spectral object encodes all of physics" — is Connes' and is not novel. Obidi is in the same conceptual family. A critic could fairly say: "You have taken Connes' move and swapped the Dirac operator for an information-geometric ratio. The architecture is the same."

The **specific implementation** is different enough to constitute genuine work, not plagiarism:
- The information-geometric foundation (Fisher-Rao, $\alpha$-connections) is a different mathematical universe from noncommutative geometry
- The ratio structure and its interpretation as "deviation from entropic equilibrium" is not in Connes
- The physical predictions (dark matter as spectral geometry, 232-as entanglement time, $c$ and $G$ as derived quantities) are not Connes' predictions

So: **not a repetition, but not a new strategy either.** It is a **new instantiation of an existing strategy**, with different mathematical foundations and different physical content. The audacity is in the scope of the claims (deriving $c$, $G$, probability conservation, the arrow of time), not in the spectral-action move itself. Connes already showed that move is viable; Obidi's challenge is to show it works with a different operator and a different ontology.


------

# Scholium 

## The Modular Operator: Where the Overlap Becomes Deepest

The search results reveal a detail that makes the Connes connection more precise — and more uncomfortable — than a surface comparison suggests. Obidi's own paper states:

> *"the G-field is reinterpreted as the modular operator Δ, whose spectral excitations manifest as entropy-driven energy density, accounting for dark matter and the small positive cosmological constant."*

And:

> *"the entropic cross-term in the Obidi Action is an Araki-type relative entropy functional over a canonical modular operator built from the entropy-weighted metric G and the reference metric g."*

This is not a loose analogy. The **Tomita–Takesaki modular operator** Δ is a specific object in operator algebra theory: given a von Neumann algebra $\mathcal{M}$ acting on a Hilbert space with a faithful normal state $\omega$, there exists a unique positive self-adjoint operator $\Delta_\omega$ (the modular operator) that encodes the **time evolution** of the algebra with respect to $\omega$. The **Araki relative entropy** $S(\rho \| \sigma) = \mathrm{Tr}(\rho \ln \rho - \rho \ln \sigma)$ is built from the logarithm of the ratio of two density operators — exactly the structure $-\mathrm{Tr}\ln(G\,g^{-1})$.

Connes' noncommutative geometry is **built on** this same mathematical structure. The spectral triple $(\mathcal{A}, \mathcal{H}, D)$ is, in a precise sense, a **modular object**: the Dirac operator $D$ is the generator of the modular flow of the algebra $\mathcal{A}$ with respect to a KMS state. The Connes–Chamseddine spectral action $\mathrm{Tr}\,f(D^2/\Lambda^2)$ is a **modular invariant** — it is computed from the spectrum of the modular operator.

So the honest statement is: **Obidi's SOA and Connes' spectral action are both built from the same mathematical object — the modular operator — but they assign it different physical meanings.** In Connes, the modular operator encodes the **geometry of spacetime and internal gauge structure**. In Obidi, the modular operator encodes the **deviation of the entropic field from equilibrium**. The mathematics is shared; the ontology is not.

This is not plagiarism. It is **convergence on a shared mathematical structure from different physical motivations**. The question is whether the convergence is deep (the mathematics *forces* this structure) or shallow (both are using the most convenient available tool).

## The dRGT Massive Gravity Lineage

There is a second, less obvious lineage that the SOA sits in. The **dRGT theory** (de Rham–Tolley–Woodard, 2010) is a bimetric gravity theory where the interaction between two metrics $g_{\mu\nu}$ and $f_{\mu\nu}$ is built from the **matrix square root** of $g^{-1}f$:

$$\mathcal{L}_{\text{int}} = \sum_{n=0}^{4} \beta_n \, \mathcal{U}_n[g^{-1}f]$$

where $\mathcal{U}_n$ are the elementary symmetric polynomials of the eigenvalues of $g^{-1}f$. The specific combination of coefficients $\beta_n$ that avoids the Boulware–Deser ghost is unique and was a major technical achievement.

Obidi's $\Delta = G[S]\,g[S]^{-1}$ is **structurally identical** to $g^{-1}f$ in dRGT: it is the ratio of two metric operators, and its eigenvalues encode the "distance" between the two geometries. The difference is:

| | dRGT | Obidi SOA |
|---|---|---|
| **Two metrics** | Ontologically separate: $g$ is physical, $f$ is reference | Two projections of the **same** entropic field |
| **Interaction** | Polynomial in eigenvalues of $g^{-1}f$ (up to 4th order) | Logarithm of the ratio: $-\mathrm{Tr}\ln(G\,g^{-1})$ |
| **Ghost freedom** | Requires specific $\beta_n$ coefficients | The log form is **automatically** ghost-free (it is the unique ghost-free function of the eigenvalues) |
| **Origin of second metric** | Postulated | Derived from the entropic field's matter-induced deformation |

The log form is not arbitrary from the dRGT perspective either. It is the **unique** function of the eigenvalues that is additive under direct sum and conformally covariant — the same properties that make it the one-loop effective action. So the SOA sits at the intersection of three lineages: **Connes' spectral action**, **dRGT bimetric gravity**, and **one-loop effective field theory**. It is not a repetition of any one of them, but it is not free of their structural constraints either.

## The "Why This Operator?" Problem

This is the most serious gap. In Connes' framework, the Dirac operator $D$ is not arbitrary. It is constrained by the **axioms of a spectral triple**:

1. $D$ is **first-order** (it commutes with the algebra $\mathcal{A}$ up to a bounded operator)
2. $D$ is **locally bounded** (its commutators with elements of $\mathcal{A}$ are bounded)
3. $D$ is **self-adjoint**
4. The algebra $\mathcal{A}$ acts **non-degenerately** on $\mathcal{H}$
5. The **real structure** $J$ satisfies $J D J^{-1} = D$ (or $-D$) and $[a, JbJ^{-1}] = 0$

These axioms are not cosmetic. They are what **force** the heat-kernel expansion to produce the Einstein–Hilbert action and the Standard Model gauge structure. Remove the first-order condition, and you get the Pati–Salam model instead of the Standard Model. Change the real structure, and you change the gauge group. The axioms are the **selection principle** that makes the spectral action work.

What are the analogous axioms for $\Delta = G[S]\,g[S]^{-1}$? From the search results, the constraints appear to be:

- $G[S]$ and $g[S]$ are **invertible** at every point on the manifold
- They are **topological** metrics (direct sums of scalar, vector, and bivector sectors)
- The ratio $\Delta$ is a **positive self-adjoint** operator (so the log is well-defined)

But this is a much weaker set of constraints than the Connes axioms. There is no first-order condition, no real structure, no non-degeneracy requirement. The result is that the SOA can be written down for **any** pair of invertible metric operators, and the heat-kernel expansion will always produce *some* geometric action. The question is: **what principle selects the specific $G[S]$ and $g[S]$ that reproduce the Standard Model?**

In Connes, the answer is: the finite spectral triple $(\mathcal{A}_F, \mathcal{H}_F, D_F)$ is **chosen** to have the representation content of the Standard Model. The choice is not derived; it is a **postulate** motivated by the observed particle content. In Obidi's framework, the equivalent question is: **what determines the specific form of the matter-induced entropy geometry $G[S]$ that encodes the Standard Model gauge group and representation content?**

The search results suggest that ToE handles this by saying that each sector (gravity, gauge, scalar, fermionic) "is governed by its own spectral Obidi action, yet all arise from the same entropic variational principle." But this is a **claim of unification**, not a **derivation**. The specific gauge group $SU(3) \times SU(2) \times U(1)$, the representation assignments, the Yukawa couplings — these are not yet shown to fall out of the SOA in the way they do in the Connes–Chamseddine–Marcolli programme. That is the critical test, and it has not yet been passed.

## The Bianconi Distinction: One Field vs. Two Metrics

The search results make the distinction between Bianconi's GfE and Obidi's ToE explicit:

> *"In Bianconi's ontology, two metrics are introduced explicitly because relative entropy requires two distributions. In ToE, the spectral Obidi Action shows that both metrics emerge as operator projections of the same entropy geometry. The 'two states' (actual vs. equilibrium entropy) are contained internally."*

This is a genuine ontological difference, not just a notational one. Bianconi's framework has **two independent metric fields** — the spacetime metric $g$ and the matter-induced metric $\tilde{G}$ — and the action is the quantum relative entropy between them. The two metrics are **independent degrees of freedom** that interact through the relative entropy term.

Obidi's claim is that this is an **illusion of duality**: $G[S]$ and $g[S]$ are not two fields but two **projections** of a single entropic field $S(x)$. The "bimetric" structure is **internal** to the entropic field, not a feature of the ontology. This is analogous to the difference between a **bimetric theory** (two independent metrics) and a **single-metric theory with an effective second metric** (where the second metric is a functional of the first and its matter content).

If Obidi is right, this is a significant simplification: the degrees of freedom are halved, and the ghost-freedom of the dRGT-type interaction becomes automatic (you cannot have a Boulware–Deser ghost in a theory with only one fundamental metric). If Obidi is wrong — if $G[S]$ and $g[S]$ are genuinely independent — then the SOA is just a **repackaging** of Bianconi's GfE with a different notation, and the "unification" is cosmetic.

## The Fermionic Sector: The Weakest Link

The search results contain a revealing sentence:

> *"Fermionic actions were always operator-spectral functionals. Bosonic actions, however, were historically local integrals. ToE's originality lies in converting bosonic actions into spectral Obidi actions, thereby unifying all sectors under one entropic-spectral principle."*

This is an honest admission. The fermionic part of the Standard Model was **already** spectral in the Connes framework — the fermionic action $(\psi, D\psi)$ is a bilinear form on the Hilbert space, and the Dirac operator $D$ is already a spectral object. The novelty of Connes' programme was to show that the **bosonic** action (gravity + gauge + Higgs) could also be written as a spectral function of the same $D$.

Obidi's claim is that he has done the equivalent: the bosonic action is now $-\mathrm{Tr}\ln(\Delta)$, and the fermionic action is a bilinear form on the same entropic Hilbert space. But the critical question is whether the **same operator** $\Delta$ that generates the bosonic action also generates the correct fermionic spectrum — the correct particle masses, mixing angles, and representation assignments. In Connes' framework, this is guaranteed by the **shared Dirac operator**: the same $D$ that gives the Einstein–Hilbert term in the heat-kernel expansion also gives the Yukawa couplings through its finite part $D_F$. In Obidi's framework, the equivalent guarantee would be that the **same** $\Delta = G[S]\,g[S]^{-1}$ that gives the gravitational action also gives the correct fermion mass matrix. This has not yet been demonstrated.

## The Verdict, Refined

The SOA is not a repetition of Connes. It is not a repetition of Bianconi. It is not a repetition of dRGT. But it is **structurally dependent** on all three, and the dependencies are not always acknowledged:

- The **modular operator** structure is shared with Connes and with the Tomita–Takesaki theory that underpins noncommutative geometry.
- The **two-metric ratio** structure is shared with Bianconi's GfE and with dRGT massive gravity.
- The **log-determinant** form is shared with one-loop effective field theory and zeta-function regularization.

The genuine novelty is in the **ontological claim** (one entropic field, not two metrics) and the **α-connection dynamics** (no Connes or dRGT analog). The genuine gap is in the **Standard Model derivation** (no equivalent of the Connes–Chamseddine–Marcolli finite spectral triple). The SOA is a real mathematical object with real physical content, but its relationship to the existing landscape is one of **convergence and recombination**, not of original invention. The audacity is in the scope of the unification claim; the provocation is in the OCP's demand that the recombination actually work.


