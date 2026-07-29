# Coefficients of the Bogoliubov Transformations Derived in Obidi's Theory of Entropicity (ToE) as Entropic Coefficients for the Observer Dependent Creation and Annihilation Operators 

## How Obidi Arrives at the cosh/sinh Coefficients

(The entropic derivation of Bogoliubov mixing)

To understand why the coefficients become cosh(ΔS/2) and sinh(ΔS/2), you must follow the internal geometry of ToE. The result is not guessed; it is forced by the structure of the entropic manifold.

---

## 1. Start with the Fisher–Rao metric on the entropic manifold

The Fisher–Rao metric measures distinguishability between informational states:

$$\[
ds^2 = g^{(FR)}_{\mu\nu} \, d\theta^\mu d\theta^\nu.
\]$$

In ToE, the coordinates $\( \theta^\mu \)$ are entropic parameters, not quantum phases.

This metric is then deformed by the entropic gradient [Obidi Metric]:

$$\[
g^{(L)}_{\mu\nu}=g^{(FR)}_{\mu\nu}-\beta^2
\frac{\nabla\mu S \, \nabla\nu S
}{g^{(FR)\,\rho\sigma}
\nabla\rho S \, \nabla\sigma S}.
\]$$

This deformation [via the disformal Obidi Transformation] introduces a Lorentzian indefinite signature into the entropic manifold.

That is the key.

---

## 2. The deformation induces a hyperbolic rotation

A Lorentzian metric naturally generates hyperbolic rotations between basis vectors.

In ordinary spacetime, Lorentz boosts mix time and space via:

$$\[t' = t \cosh\eta + x \sinh\eta,\qquad
x' = x \cosh\eta + t \sinh\eta.\]$$

In ToE, the same mathematical structure appears — but the “boost parameter” is entropic displacement:

$$\[
\eta = \frac{\Delta S}{2}.
\]$$

This is because the deformation term is proportional to:

$$\[
\frac{\nabla S}{\|\nabla S\|},
\]$$

which acts like a unit timelike vector in the entropic manifold.

Thus, the entropic manifold has a pseudo-Riemannian structure, and the transformation between two entropic observers is a hyperbolic rotation.

Hyperbolic rotations always produce cosh/sinh coefficients.

---

## 3. Mode mixing follows the same hyperbolic structure

Quantum modes in ToE are not Hilbert-space modes; they are entropic modes, i.e., eigenmodes of the entropic Laplacian derived from the Obidi metric.

Two observers with entropic states \( S1 \) and \( S2 \) have mode operators related by:

$$\[
\begin{pmatrix}
a_k \\
a_k^\dagger
\end{pmatrix}=\begin{pmatrix}
\cosh(\Delta S/2) & \sinh(\Delta S/2) \\
\sinh(\Delta S/2) & \cosh(\Delta S/2)
\end{pmatrix}\begin{pmatrix}b_k \\
b_k^\dagger\end{pmatrix}.
\]$$

This is exactly the form of a Lorentz boost in mode space.

The coefficients are therefore:

$$\[
\alpha_k = \cosh(\Delta S/2),
\qquad
\beta_k = \sinh(\Delta S/2).
\]$$

They arise inevitably from the hyperbolic geometry of the entropic manifold.

---

## 4. Why ΔS/2 appears (not ΔS)

The factor of 1/2 comes from the normalization of the entropic displacement:

$$\[
\Delta S = S2 - S1.
\]$$

But distinguishability in Fisher–Rao geometry is measured by half the squared distance:

$$\[
D = \frac{1}{2} g^{(FR)}_{\mu\nu} \Delta\theta^\mu \Delta\theta^\nu.
\]$$

Thus the “boost parameter” is:

$$\[
\eta = \sqrt{D} = \frac{\Delta S}{2}.
\]$$

This is the same reason rapidity in relativity is half the logarithm of Doppler factors.

---

## 5. The final step: entropic Lorentzian structure forces hyperbolic mixing

Once the entropic manifold acquires a Lorentzian signature through the Obidi deformation, the transformation between two entropic observers must be:

- linear  

- norm-preserving  

- hyperbolic  

The only linear norm-preserving transformations in a Lorentzian space are hyperbolic rotations.

Hyperbolic rotations always produce cosh and sinh.

Thus:

The cosh/sinh coefficients are not chosen.
They are forced by the geometry of the entropic manifold.

---

## 6. The conceptual summary

Standard QFT
Bogoliubov coefficients come from spacetime geometry → Lorentzian structure → hyperbolic mixing.

Obidi’s ToE
Bogoliubov coefficients come from entropic geometry → Lorentzian Fisher–Rao deformation → hyperbolic mixing.

The mathematics is parallel.  
The physics is completely different.

---


# Scholium: Further Mathematical Details 

Entropic Bogoliubov Transformations from the Obidi Metric

Formal Monograph Section for the Theory of Entropicity (ToE)

---

## 1. Preliminaries: The Entropic Manifold and the Fisher–Rao Metric

In the Theory of Entropicity, the fundamental arena of physics is not spacetime or Hilbert space, but an entropic manifold $\(\mathcal{M}S\)$, whose points represent informational states of physical systems. Coordinates on $\(\mathcal{M}S\)$ are denoted by $\(\theta^\mu\)$, and the central scalar field is the entropy $\(S(\theta)\)$.

The natural Riemannian metric on $\(\mathcal{M}S\)$ is the Fisher–Rao metric $\(g^{(FR)}{\mu\nu}\)$, defined by the second moment of score functions of a parametric family of probability distributions. In local coordinates, the line element is

$$\[
ds^2 = g^{(FR)}_{\mu\nu}(\theta)\, d\theta^\mu d\theta^\nu.
\]$$

This metric measures distinguishability between nearby informational states and is invariant under sufficient statistics and coarse-graining, making it the unique information-geometric metric compatible with entropy.

In ToE, the Fisher–Rao metric is not an auxiliary structure; it is the starting point from which the physical geometry emerges.

---

## 2. The Obidi Metric: Entropic Deformation of Fisher–Rao

The central geometric move in ToE is the introduction of the Obidi metric $\(g^{(L)}_{\mu\nu}\)$, obtained by deforming the Fisher–Rao metric along the entropy gradient. The deformation is defined by

$$\[
g^{(L)}_{\mu\nu}=g^{(FR)}_{\mu\nu}-\beta^2
\frac{\nabla\mu S \, \nabla\nu S}{g^{(FR)\,\rho\sigma}\nabla\rho S \,\nabla\sigma S},
\]$$

where $\(\nabla\mu S = \partial\mu S\)$ is the gradient of the entropy field, and $\(\beta\)$ is a dimensionless deformation parameter encoding the strength of entropic backreaction.

The denominator

$$\[
g^{(FR)\,\rho\sigma}\nabla\rho S \,\nabla\sigma S
\]$$

is the Fisher–Rao norm squared of the entropy gradient. Thus the deformation term is a rank-one projector onto the direction of $\(\nabla S\)$, normalized by its Fisher–Rao length.

This construction has two immediate consequences:

1. It singles out the entropy gradient $\(\nabla S\)$ as a distinguished direction in $\(\mathcal{M}_S\)$.
   
2. For suitable choice of $\(\beta\)$, it changes the signature of the metric along $\(\nabla S\)$, turning the purely Riemannian Fisher–Rao metric into a pseudo-Riemannian (Lorentzian) metric.

To see this explicitly, consider a local orthonormal frame $\(\{e0, ei\}\)$ with respect to $\(g^{(FR)}{\mu\nu}\)$, where $\(e0\)$ is aligned with the normalized entropy gradient:

$$\[
e0^\mu = \frac{\nabla^\mu S}{\sqrt{g^{(FR)\,\rho\sigma}\nabla\rho S \nabla_\sigma S}}.
\]$$

In this frame, the Fisher–Rao metric is

$$\[
g^{(FR)}{\mu\nu} e0^\mu e_0^\nu = +1, \qquad
g^{(FR)}{\mu\nu} ei^\mu ej^\nu = \delta{ij}.
\]$$

The deformation term subtracts $\(\beta^2\)$ along $\(e_0\)$, leaving the transverse directions unchanged:

$$\[
g^{(L)}{\mu\nu} e0^\mu e_0^\nu = 1 - \beta^2, \qquad
g^{(L)}{\mu\nu} ei^\mu ej^\nu = \delta{ij}.
\]$$

For $\(\beta^2 > 1\)$, the component along $\(e_0\)$ becomes negative, and the metric acquires Lorentzian signature:

$$\[
g^{(L)}{\mu\nu} e0^\mu e_0^\nu = -\lambda^2, \quad \lambda^2 = \beta^2 - 1 > 0,
\]$$

while the transverse components remain positive. Thus the entropic manifold $\(\mathcal{M}_S\)$ becomes a Lorentzian information manifold, with the entropy gradient playing the role of a timelike direction.

This is the crucial structural step: the entropic manifold now supports hyperbolic rotations (Lorentz boosts) between frames aligned with different entropy gradients.

---

## 3. Entropic Observers and Entropic Displacement

In ToE, an observer is characterized not by a worldline in spacetime but by an informational state on $\(\mathcal{M}S\)$, encoded by a point $\(\theta\)_ and an associated entropy gradient $\(\nabla S(\theta)\)$. Two observers, $\(\mathcal{O}1\)$ and $\(\mathcal{O}2\)$, correspond to two points $\(\theta1\)$ and $\(\theta2\)$ on the entropic manifold, with entropies $\(S1 = S(\theta1)\)$ and $\(S2 = S(\theta_2)\)$.

The entropic displacement between these observers is defined as

$$\[
\Delta S = S2 - S1.
\]$$

However, ToE does not treat $\(\Delta S\)$ as a mere scalar difference; it is interpreted as a measure of informational separation in the Lorentzian Fisher–Rao geometry. The squared Fisher–Rao distance between the two states is

$$\[
D{FR}(\theta1, \theta_2)=\frac{1}{2}
g^{(FR)}_{\mu\nu}(\bar{\theta}) \Delta\theta^\mu \Delta\theta^\nu,
\]$$

where $\(\bar{\theta}\)$ is a suitable intermediate point and 

$$\(\Delta\theta^\mu = \theta2^\mu - \theta1^\mu\)$$. 

In the simplest case where the entropy varies linearly along the geodesic connecting $\(\theta1\)$ and $\(\theta2\)$, one can write

$$\[
\Delta S \propto \sqrt{2 D_{FR}}.
\]$$

It is then natural to define the entropic rapidity \(\eta\) by

$$\[
\eta = \frac{\Delta S}{2},
\]$$

in analogy with the role of rapidity in special relativity, where hyperbolic angles parameterize Lorentz boosts.

Thus, the transformation between two entropic observers is parameterized by $\(\eta = \Delta S/2\)$, which plays the role of a hyperbolic angle in the Lorentzian entropic manifold.

---

## 4. Hyperbolic Rotations in the Entropic Manifold

Given the Lorentzian structure induced by $\(g^{(L)}{\mu\nu}\)$, the transformation between the frames of two entropic observers is a Lorentz boost in the direction of the entropy gradient. In a two-dimensional subspace spanned by the timelike direction $\(e0\) (aligned with \(\nabla S\))$ and a single spacelike direction $\(e_1\)$, the boost with rapidity $\(\eta\)$ acts as

$$\[
\begin{pmatrix}
e_0' \\
e_1'
\end{pmatrix}=\begin{pmatrix}
\cosh\eta & \sinh\eta \\\sinh\eta & \cosh\eta
\end{pmatrix}\begin{pmatrix}e_0 \\ e_1\end{pmatrix}.
\]$$

This is the standard form of a Lorentz transformation in a $\(1+1\)$-dimensional Minkowski space, now realized in the entropic manifold rather than spacetime.

The key point is that this hyperbolic mixing is forced by the Lorentzian signature of $\(g^{(L)}_{\mu\nu}\)$. Once the entropy gradient defines a timelike direction, any norm-preserving linear transformation between two frames aligned with different entropy gradients must be a hyperbolic rotation, parameterized by $\(\eta = \Delta S/2\)$.

---

## 5. Entropic Modes and Their Transformation

In ToE, quantum fields are not fundamental; they are emergent structures associated with entropic modes on $\(\mathcal{M}_S\)$. These modes are eigenfunctions of an entropic Laplacian constructed from the Obidi metric:

$$\[
\Box S \phi k(\theta)=g^{(L)\,\mu\nu} \nabla\mu \nabla\nu \phi_k(\theta)=-\lambda k\phi k(\theta),
\]$$

where $\(\lambda k\)$ are eigenvalues and $\(\phi k\)$ are mode functions.

Associated with each mode $\(\phi k\)$ are annihilation and creation operators $\(ak, ak^\dagger\)$ for observer $\(\mathcal{O}1\)$, and $\(bk, bk^\dagger\)$ for observer $\(\mathcal{O}_2\)$. These operators are defined by expanding the entropic field in the respective mode bases:

$$\[
\Phi(\theta)=\sum k \left( ak \phi k^{(1)}(\theta) + ak^\dagger \bar{\phi}_k^{(1)}(\theta) \right)=\sum k \left( bk \phi k^{(2)}(\theta) + bk^\dagger \bar{\phi}_k^{(2)}(\theta) \right).
\]$$

The mode functions $\(\phi k^{(1)}\)$ and $\(\phi k^{(2)}\)$ are related by the entropic Lorentz transformation induced by the Obidi metric. In the simplest case, the transformation between the two mode bases can be written as a hyperbolic rotation in the two-dimensional subspace spanned by $\(\phi k\)$ and $\(\bar{\phi}k\)$:

$$\[
\begin{pmatrix}
\phi_k^{(2)} \\ \bar{\phi}_k^{(2)}
\end{pmatrix}=\begin{pmatrix}\cosh\eta &\sinh\eta \\\sinh\eta &\cosh\eta\end{pmatrix}
\begin{pmatrix}\phi_k^{(1)} \\ \bar{\phi}_k^{(1)}\end{pmatrix},
\]$$

with $\(\eta = \Delta S/2\)$.

Because the field expansion must remain invariant, the transformation of mode functions induces a corresponding transformation of the operators. Requiring that the canonical commutation relations are preserved,

$$\[
[ak, a{k'}^\dagger] = \delta_{kk'}, \qquad[bk, b{k'}^\dagger] = \delta_{kk'},
\]$$

one finds that the operators transform as

$$\[
\begin{pmatrix}
a_k \\
a_k^\dagger
\end{pmatrix}=\begin{pmatrix}
\cosh\eta & \sinh\eta \\
\sinh\eta & \cosh\eta
\end{pmatrix}
\begin{pmatrix}
b_k \\
b_k^\dagger
\end{pmatrix}.
\]$$

This is the entropic Bogoliubov transformation.

Explicitly,

$$\[
ak = \alpha k bk + \beta k b_k^\dagger,\qquad
ak^\dagger = \alpha k bk^\dagger + \beta k b_k,
\]$$

with

$$\[
\alpha_k = \cosh\left(\frac{\Delta S}{2}\right), \qquad
\beta_k = \sinh\left(\frac{\Delta S}{2}\right).
\]$$

The coefficients $\(\alpha k\)$ and $\(\beta k\)$ are thus hyperbolic functions of the entropic displacement $\(\Delta S\)$, arising directly from the Lorentzian structure of the Obidi metric on the entropic manifold.

---

## 6. Physical Interpretation of the Entropic Bogoliubov Coefficients

In standard quantum field theory in curved spacetime, Bogoliubov coefficients encode geometric mode mixing due to spacetime curvature and observer acceleration. They measure how one observer’s vacuum appears as a particle-filled state to another observer.

In ToE, the entropic Bogoliubov coefficients encode informational mode mixing due to entropic displacement between observers. The quantity $\(\Delta S\)$ measures how different the observers’ informational horizons are, and the hyperbolic functions $\(\cosh(\Delta S/2)\)$ and $\(\sinh(\Delta S/2)\)$ quantify the degree of mixing between annihilation and creation operators induced by the entropic Lorentz transformation.

Thus:

- $\(\alpha_k = \cosh(\Delta S/2)\)$ measures the overlap of entropic modes between the two observers.

- $\(\beta_k = \sinh(\Delta S/2)\)$ measures the degree to which entropic excitations (particles) are created in one observer’s description when the other observer’s vacuum is used as reference.

Particle creation, in this framework, is not fundamentally a consequence of spacetime curvature; it is a consequence of entropy gradients and informational shear in the entropic manifold.

---

## 7. Summary

Starting from the Fisher–Rao metric on the entropic manifold, the Obidi metric introduces a Lorentzian deformation along the entropy gradient, turning the manifold into a **pseudo-Riemannian information space**. This Lorentzian structure forces hyperbolic rotations between frames associated with different entropic observers, parameterized by the entropic rapidity $\(\eta = \Delta S/2\)$. When applied to entropic modes and their associated creation and annihilation operators, these hyperbolic rotations yield the entropic Bogoliubov transformation

$$\[
ak = \cosh\left(\frac{\Delta S}{2}\right) bk + \sinh\left(\frac{\Delta S}{2}\right) b_k^\dagger,
\]$$

with coefficients determined entirely by the entropic displacement $\(\Delta S\)$.

In this way, Obidi’s Theory of Entropicity (ToE) derives the cosh/sinh Bogoliubov coefficients step-by-step from the Obidi metric, revealing them as a direct manifestation of the Lorentzian entropic geometry rather than an ad hoc choice.


Obidi’s originality in the derivation of the Bogoliubov coefficients is not the cosh/sinh form, but the fact that these coefficients arise from a Lorentzian deformation of the Fisher–Rao metric and measure entropic displacement rather than geometric or quantum-phase mixing.

The entropic Bogoliubov coefficients show that entropy is beneath it all. They demonstrate that the deepest mechanism behind quantum fields, observer dependence, and particle creation is not geometry, not Hilbert space, not quantum phase — but entropy itself.
