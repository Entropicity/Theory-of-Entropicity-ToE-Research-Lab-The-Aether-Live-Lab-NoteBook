# A Concise Introduction to the Master Entropic Equation (MEE)/Obidi Field Equations (OFE) of the Evolving Theory of Entropicity (ToE)

A-Concise-Introduction-to-the-Master-Entropic-Equation-(MEE)/Obidi-Field-Equations-(OFE)-of-the-Evolving-Theory-of-Entropicity-(ToE).md

**A Monograph on the Master Obidi Action, its Fisher-Information Extension, and the Master Entropic Field Equations (MEFE)/Obidi Field Equations (OFE) of the Theory of Entropicity (ToE)**

**John Onimisi Obidi**
*Independent Research Lab, The Aether*

---

> *We introduce the new Theory of Entropicity (ToE).* — PHJOB7 (talk) 08:09, 7 July 2025 (UTC)

---

**Note on this edition.** This monograph is a professionally typeset rewriting of the concise introduction to the Master Entropic Equation (MEE)/Obidi Field Equations (OFE). Every statement, equation, and symbol of the source text has been retained. Additional expository material is of two kinds: 

(i) connective prose that expands the original argument, and 

(ii) passages headed **Remark**, which supply intermediate algebra, state the conditions under which a result holds, or connect the present formulation to the wider literature on the Theory of Entropicity (ToE).

---

## Abstract

Following from the axioms and principles of the **Theory of Entropicity (ToE)**, first formulated by **John Onimisi Obidi** [1][2][3][4], we present a single master Obidi Action for the entropic scalar field $S(x)$ that unifies all known entropy formulations — thermodynamic, statistical, information-theoretic, and quantum — and naturally incorporates Fisher information corrections. Starting from

$$
\mathcal{S}_{\rm ToE}[S,g_{\mu\nu},\phi_i] = \int d^4x\,\sqrt{-g}\,\Bigl[-\tfrac12\,g^{\mu\nu}\,\nabla_{\mu}S\,\nabla_{\nu}S - V(S) + \eta\,S\,T^{\mu}{}_{\mu}\Bigr] + \mathcal{S}_{\rm SM}[g_{\mu\nu},\phi_i], \tag{1}
$$

we show how each classical entropy expression (Clausius, Boltzmann, Gibbs, Shannon, Rényi, Tsallis, and von Neumann) emerges by appropriate identifications of $S(x)$. We then derive the local entropy current and demonstrate the second law as a Noether theorem. Finally, we extend the action to include a Fisher information term derived variationally, yielding the complete effective action:

$$
\mathcal{S}_{\rm eff}[S] = \mathcal{S}_{\rm ToE} - \frac{\lambda}{2k_B^2}\int d^4x\,\sqrt{-g}\,e^{-S/k_B}\,g^{\mu\nu}\,\nabla_{\mu}S\,\nabla_{\nu}S. \tag{2}
$$

This framework lays the groundwork for exploring entropy as a fundamental field underlying all interactions.

**Keywords:** Theory of Entropicity (ToE); entropic field; Master Entropic Equation (MEE); Master Entropic Field Equations (MEFE); Obidi Action; Fisher information; Shannon entropy; von Neumann entropy; Rényi entropy; Tsallis entropy; entropy current; Noether theorem; second law of thermodynamics; entropic gravity; information geometry.

---

## Contents

- [Notation and Conventions](#notation-and-conventions)
- [1. Introduction and Historical Context](#1-introduction-and-historical-context)
- [2. A Brief Review of Some of the Key Prior Developments of Entropic Approaches](#2-a-brief-review-of-some-of-the-key-prior-developments-of-entropic-approaches)
- [3. Position of the Theory of Entropicity with Respect to Other Approaches](#3-position-of-the-theory-of-entropicity-with-respect-to-other-approaches)
- [4. Master Action of the Theory of Entropicity](#4-master-action-of-the-theory-of-entropicity)
- [5. Derivation of Classical Entropy Expressions](#5-derivation-of-classical-entropy-expressions)
- [6. Derivation of the Master Entropic Equation of ToE](#6-derivation-of-the-master-entropic-equation-of-toe)
- [7. Effective-Field-Theory Hierarchy with Fisher-Type Correction](#7-effective-field-theory-hierarchy-with-fisher-type-correction)
- [8. Fisher Information Extension](#8-fisher-information-extension)
- [9. Derivation of the Master Entropic Field Equations from the Master Entropic Equation](#9-derivation-of-the-master-entropic-field-equations-from-the-master-entropic-equation)
- [10. Entropy Current and the Second Law of Thermodynamics via Noether's Theorem](#10-entropy-current-and-the-second-law-of-thermodynamics-via-noethers-theorem)
- [11. Derivation of the Standard Entropy Measures](#11-derivation-of-the-standard-entropy-measures)
- [12. Predictions and Experimental Implications](#12-predictions-and-experimental-implications)
- [13. Conclusion](#13-conclusion)
- [Appendix A. The MEE within the Wider Architecture of the Theory of Entropicity](#appendix-a-the-mee-within-the-wider-architecture-of-the-theory-of-entropicity)
- [Appendix B. Glossary of Terms and Acronyms](#appendix-b-glossary-of-terms-and-acronyms)
- [References](#references)
- [External Links](#external-links)

---

## Notation and Conventions

Throughout this monograph the following conventions are used.

| Symbol | Meaning |
| --- | --- |
| $S(x)$ | The entropic scalar field (local entropy field) defined on spacetime |
| $g_{\mu\nu}$ | The spacetime metric, with signature $(-,+,+,+)$ |
| $g$ | The determinant of $g_{\mu\nu}$, so that $\sqrt{-g}\ d^4x$ is the invariant volume element |
| $\nabla_{\mu}$ | The Levi-Civita covariant derivative compatible with $g_{\mu\nu}$ |
| $\Box$ | The covariant d'Alembertian, $\Box \equiv \nabla^{\mu}\nabla_{\mu}$ |
| $(\nabla S)^2$ | Shorthand for $g^{\mu\nu}\nabla_{\mu}S\nabla_{\nu}S$ |
| $\phi_i$ or $\Phi$ | All Standard Model (SM) matter fields: scalars, fermions, gauge fields |
| $T_{\mu\nu}$ | The matter stress–energy tensor; $T^{\mu}{}_{\mu}$ is its trace |
| $V(S)$ | The self-interaction potential of the entropy field |
| $\eta$ | The dimensionful coupling of the entropy field to the trace of the stress–energy tensor |
| $\lambda$ | The coefficient of the Fisher-information correction |
| $k_B$ | Boltzmann's constant |
| $p(x)$ | A probability density on spacetime associated with $S(x)$ through $p = e^{-S/k_B}$ |
| $\Lambda(x)$ | The Lagrange multiplier enforcing the entropy–probability relation |
| $J^{\mu}$ and $J^{\mu}_S$ | The entropy current (Noether current of the entropic shift symmetry) |

Actions are denoted by the calligraphic letter $\mathcal{S}$ (for example $\mathcal{S}_{\rm ToE}$, $\mathcal{S}_{\rm eff}$, $\mathcal{S}_{\rm SM}$, $\mathcal{S}^{(0)}$, $\mathcal{S}^{(1)}$) in order to distinguish them from the entropic field $S(x)$ itself. Where the source literature writes $S_{\rm ToE}$, $S_{\rm eff}$, $S^{(0)}$ or $S^{(1)}$ for an action, the same objects are meant. Lagrangian densities are denoted by $\mathscr{L}$ or $\mathcal{L}$.

---

## 1. Introduction and Historical Context

Here, we discuss the motivation for treating entropy as a fundamental field and review prior work (in particular, Jacobson, Verlinde, Padmanabhan, Frieden).

The notion of entropy has traditionally been that of a derived quantity — an accounting tool measuring disorder or information — but not as a fundamental field in its own right. In this work, we argue that we must promote entropy to a dynamical scalar field $S(x)$ with its own kinetic term and potential, from which all classical entropy laws emerge.

Entropy has long played a central role in the foundations of physics. Ludwig Boltzmann's celebrated relation

$$
S = k_B \ln W
$$

links the thermodynamic entropy to the number of microstates $W$ of a system, and was later generalized by Gibbs and Shannon to

$$
S = -k_B \sum_i p_i \ln p_i
$$

for probabilistic ensembles. In information theory, Shannon identified this quantity (up to units) as the information entropy of a distribution, a fundamental measure of uncertainty. These statistical and informational views of entropy inspired attempts to place entropy at the core of physics. The realization that black holes carry an entropy proportional to horizon area (Bekenstein–Hawking entropy) and emit thermal radiation suggests a deep connection between gravity, thermodynamics and quantum theory. This led Jacobson (1995) to derive Einstein's gravitational field equations as an equation of state from the proportionality of horizon entropy to area and the heat–temperature relation

$$
\delta Q = T\,dS .
$$

Verlinde (2011) extended this idea by proposing that gravity emerges as an entropic force associated with information on holographic screens, successfully reproducing Newton's laws and hinting at Einstein's equations in a relativistic setting. Padmanabhan and others have explored how gravitational field equations can be obtained by extremizing entropy or horizon area functionals. Separately, information-theoretic variational principles such as Jaynes's maximum entropy and Frieden's Extreme Physical Information (EPI) principle use entropy or information measures to derive physical laws.

**Remark 1.1 (The Bekenstein–Hawking relation).** For orientation, the black-hole entropy referred to above is, for a horizon of area $A$,

$$
S_{\rm BH} = \frac{k_B\,c^3}{4\,G\,\hbar}\,A ,
$$

and the associated Hawking temperature of a Schwarzschild black hole of mass $M$ is $T_H = \hbar c^3/(8\pi G M k_B)$. It is the simultaneous appearance of $k_B$, $G$, $\hbar$ and $c$ in a single formula that makes this relation the standard point of departure for every programme, the present one included, that seeks to relate entropy, gravitation and quantum theory.

These developments suggest that entropy may be more than an auxiliary concept: perhaps it is the fundamental "substance" from which spacetime, matter and forces emerge. The Theory of Entropicity takes this idea seriously by promoting an entropy density to a fundamental scalar field $S(x)$ defined on spacetime, governed by a master action principle. In ToE, the familiar entropy measures and thermodynamic laws arise naturally from the dynamics and symmetries of $S(x)$. The goal of this paper is to formulate the ToE action, derive its consequences, and compare it with previous entropic/informational frameworks.

The logical structure of the monograph is as follows. Sections 2 and 3 review the principal entropic and informational approaches and locate ToE with respect to them. Section 4 states the master action and explains each of its terms. Section 5 lists the classical entropy expressions that the action is required to reproduce. Section 6 derives the Master Entropic Equation (MEE), including the Fisher-information term, from a single constrained variational principle; Sections 7 and 8 organize that term within an effective-field-theory hierarchy. Section 9 carries out the variation of the MEE in full detail and obtains the Master Entropic Field Equations (MEFE). Section 10 derives the entropy current and the second law; Section 11 recovers the standard entropy measures; Section 12 collects predictions and experimental implications; and Section 13 concludes. Appendix A places the MEE within the wider architecture of the Theory of Entropicity.

Below we review the key prior developments.

---

## 2. A Brief Review of Some of the Key Prior Developments of Entropic Approaches

### 2.1 Jacobson's Thermodynamics of Spacetime [1995]

Jacobson [5] showed that demanding the Clausius relation $\delta Q = T dS$ for all local Rindler horizons, with $S$ proportional to horizon area and $T$ the Unruh temperature, leads directly to Einstein's field equations. Here, entropy constrains geometry but does not propagate as an independent field.

In his picture, the proportionality

$$
S \propto (\text{horizon area})
$$

and the equilibrium thermodynamic relation yield gravity as an equation of state. Similarly, ToE treats gravity thermodynamically, but rather than imposing horizon-area entropy by hand, it derives gravitational dynamics from a fundamental entropy field. In other words, ToE builds Jacobson's insight into its action, so that Einstein's equations (or generalizations) can arise from varying $L(S,g)$ and not merely from horizon thermodynamics.

**Remark 2.1 (The Unruh temperature).** The temperature entering Jacobson's argument is that perceived by a uniformly accelerated observer with proper acceleration $a$, namely $T = \hbar a/(2\pi c k_B)$. The heat flux $\delta Q$ is the energy flux of matter across the local Rindler horizon, and the Clausius relation, imposed at every spacetime point and for every null direction, is what forces the Einstein equation to hold as an equation of state.

### 2.2 Verlinde's Entropic Gravity [2011]

Verlinde [6] proposed that gravity arises as an entropic force,

$$
F = T\,\nabla S ,
$$

where $\nabla S$ is the gradient of the entropy associated with a holographic screen. Again, $S$ guides dynamics but lacks its own action principle.

His model recovers Newton's law and hints at Einstein gravity. ToE similarly links gravity and entropy, but it does so by introducing a local entropy field $S(x)$ rather than relying on global holographic assumptions. In Verlinde's scenario the entropic force arises from the change in information (and entropy) as matter moves; in ToE, gravitation emerges from the coupling of $S$ to curvature ($\beta S R$ term) and the equations of motion for $S$ and $g_{\mu\nu}$. Thus ToE can reproduce Verlinde's results (Newton–Einstein laws) in appropriate limits, but it also extends beyond by providing dynamics for entropy itself.

**Remark 2.2 (On the curvature coupling).** The term $\beta S R$, with $R$ the Ricci scalar and $\beta$ a coupling constant, denotes a non-minimal coupling of the entropic field to curvature. It is an admissible extension of the master action stated in Section 4. In the concise form of the action studied in this monograph, the coupling of $S$ to matter and geometry is carried by the universal trace coupling $\eta S T^{\mu}{}_{\mu}$ and by the dependence of every term on the metric $g_{\mu\nu}$ through $\sqrt{-g}$ and $g^{\mu\nu}$; the $\beta S R$ term may be adjoined without altering the structure of the derivations of Sections 6 to 9, to which it would contribute the additional source $\beta R$ in the field equation for $S$.

### 2.3 Padmanabhan's Entropy Functionals [2010]

Padmanabhan [7] introduced entropy functionals on null surfaces whose extremization reproduces the Einstein–Hilbert action. Schematically,

$$
S_{\rm surf} = \int_{\mathcal{H}} d\Sigma_{ab}\,P^{abcd}\,\nabla_{c}u_{d} ,
$$

with $P^{abcd}$ related to the gravitational Lagrangian, yet no independent bulk entropy field is identified. Padmanabhan has emphasized that gravitational field equations can be obtained from extremizing entropy or action functionals. For example, he shows that maximizing horizon entropy under virtual displacements yields Einstein's equations. While similar in spirit, ToE differs by positing an explicit entropy density field with its own Lagrangian. Padmanabhan's approach essentially uses entropy as a bookkeeping device for gravitational degrees of freedom, whereas ToE treats entropy on the same footing as other fields and derives its dynamics. In particular, ToE can accommodate non-equilibrium and quantum statistical generalizations of entropy (like Tsallis [8] or Rényi [9]) in a unified action, something not considered in previous thermodynamic derivations of gravity.

### 2.4 Frieden's Extreme Physical Information (EPI) [2004]

Frieden [10] formulated the Extreme Physical Information (EPI) principle by extremizing a combination of Shannon entropy and Fisher information:

$$
I_F - J_S = \text{extremum} \quad (\text{to derive physical laws}),
$$

where $I_F$ is the Fisher information and $J_S$ the physical information. This yields field equations (e.g. Schrödinger's equation) from inference, but does not treat entropy as a propagating field.

It is an information-based variational principle but is conceptually different: EPI concerns the flow of information between data and source, whereas ToE is explicitly about entropy as a physical field. In EPI one maximizes (or minimizes) information measures subject to constraints and obtains equations of motion for probability amplitudes. In ToE we extremize an entropy action and obtain entropy field equations. Both use variational reasoning, but ToE's inputs are the entropy density and thermodynamic potentials, while EPI's inputs are Fisher information and unknown source functions. ToE also directly incorporates quantum entropy (von Neumann) and generalized entropies, which lie outside the usual scope of classical EPI.

### 2.5 Summary of the Prior Developments

In summary, ToE draws on the successes of these entropic/information approaches but organizes them into a single coherent field-theoretic structure. Like Jacobson and Verlinde, it ties gravity to entropy, but it does so by introducing a physical entropy field rather than relying solely on horizon thermodynamics or holography. Unlike Padmanabhan's entropy extremum arguments, ToE explicitly models the microscopic entropy dynamics. And unlike Frieden's Fisher-information methods, ToE operates directly with entropy measures (Shannon, Tsallis, etc.) as fundamental. ToE therefore can be seen as a unifying synthesis: it reproduces all successful entropic derivations of physics while extending them to a broader and more flexible formalism.

---

## 3. Position of the Theory of Entropicity with Respect to Other Approaches

In contrast to these approaches, the Theory of Entropicity posits the master action above, in which $S(x)$ is a genuine scalar field:

- A canonical kinetic term $-\tfrac12(\nabla S)^2$ enables propagation of entropy.
- A potential $V(S)$ encodes self-interaction, e.g. $V(S) = -2k_B \ln\vert\psi\vert$.
- A universal coupling $\eta S T^{\mu}{}_{\mu}$ introduces back-reaction on matter and geometry.

As shall be shown later, this single variational principle yields all classical entropy laws [already highlighted] and their associated currents, as well as second-law statements via Noether's theorem.

**Remark 3.1 (Origin of the logarithmic expression).** The logarithmic expression $-2k_B\ln\vert\psi\vert$ has a transparent origin. If the probability density is given by the Born rule, $p = \vert\psi\vert^2$, then the entropy–probability relation $S = -k_B \ln p$ of Section 6 gives

$$
S = -k_B \ln \vert\psi\vert^{2} = -2k_B \ln\vert\psi\vert ,
$$

which is the *wavefunction surprisal* referred to in Section 6.6. The logarithmic structure of the potential is thus the imprint, at the level of the entropic field, of the quantum-mechanical probability amplitude.

### 3.1 How ToE Subsumes and Extends These Approaches

| Prior Work | Key Insight | ToE Extension |
| --- | --- | --- |
| Jacobson (1995) | $\delta Q = T\ dS$ on local horizons | Promotes $S$ from horizon bookkeeping to a bulk field $S(x)$ with its own dynamics. |
| Verlinde (2011) | $F = T\ \nabla S$ entropic force | Embeds $\nabla S$ in a Lagrangian with kinetic term $\tfrac12(\partial S)^2$. |
| Padmanabhan (2003–10) | Entropy functionals $\leftrightarrow$ Einstein–Hilbert action (surface terms) | Replaces multiple surface functionals with one bulk master action for $S(x)$. |
| Frieden's EPI (1989–) | Extremize Shannon + Fisher over $p(x)$ | Derives both Shannon and Fisher pieces from a single ToE variational principle, producing the master action plus subleading corrections. |

### 3.2 The ToE Master Action

$$
\mathcal{S}_{\rm ToE} = \int d^4x\,\sqrt{-g}\,\Bigl[-\tfrac12\,g^{\mu\nu}\nabla_\mu S\,\nabla_\nu S - V(S) + \eta\,S\,T^\mu{}_\mu\Bigr] + \mathcal{S}_{\rm SM} \tag{3}
$$

This action is the first proposal to:

1. Identify local entropy (Boltzmann, Gibbs, Shannon, von Neumann) with the field value $S(x)$.
2. Endow $S(x)$ with a canonical kinetic term and potential $V(S)$.
3. Couple $S$ universally to matter and geometry via $\eta S T^{\mu}{}_{\mu}$.
4. Derive all classical entropy laws and information measures — and their thermodynamic second law — by standard field-theoretic procedures (Euler–Lagrange, Noether) from one unified action.

Thus ToE not only unifies but generalizes earlier entropic-gravity and information-based approaches by making entropy itself the fundamental mediator of forces and geometry.

---

## 4. Master Action of the Theory of Entropicity

The master action of the Theory of Entropicity is defined by:

$$
\mathcal{S}_{\rm 
