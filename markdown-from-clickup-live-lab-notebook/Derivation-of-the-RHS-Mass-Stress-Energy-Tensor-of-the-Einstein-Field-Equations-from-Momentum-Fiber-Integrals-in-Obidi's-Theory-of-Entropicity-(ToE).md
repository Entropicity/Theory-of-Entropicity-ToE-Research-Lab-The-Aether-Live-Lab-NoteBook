# Derivation of the RHS [Mass Stress-Energy Tensor] of the Einstein Field Equations from Momentum Fiber Integrals in Obidi's Theory of Entropicity (ToE) 

## Core idea
Obidi’s derivation did not consist of integrating entropy $\(S\)$ directly and declaring the result to be $\(T_{\mu\nu}\)$. A scalar fiber integral would still be a scalar and could not supply the rank-two tensor required on the right-hand side of Einstein’s field equations.

Instead, he constructed a rank-two entropic stress kernel on the full entropic-information bundle and then integrated that kernel over the internal fibers. The resulting tensor on emergent spacetime was identified with the effective matter stress-energy tensor.

The logical chain was

$\[
\text{Entropic microstates}
\longrightarrow
\text{entropic momentum and stress}
\longrightarrow
\text{rank-two fiber moment}
\longrightarrow
T_{\mu\nu}^{(\mathrm{ent})}
\longrightarrow
\frac{8\pi G}{c^{4}}T_{\mu\nu}.
\]$


---

1. The entropic fiber bundle

Obidi begins with a bundle

$\[
\pi:\mathcal E\longrightarrow \mathcal M,
\]$

where:

$\(\mathcal M\)$ is the emergent Lorentzian spacetime manifold;

$\(\mathcal E\)$ is the total entropic-information space;

$\(\mathcal F_x=\pi^{-1}(x)\)$ is the fiber over the spacetime event $\(x\)$;

$\(\zeta\in\mathcal F_x\)$ labels internal entropic, informational, spectral, statistical, or quantum states.


A point in the total space is therefore written schematically as

$\[
(x,\zeta)\in\mathcal E
\]$.

The entropic field is not merely a spacetime scalar $\(S(x)\)$, but may be represented more completely as

$\[
S=S(x,\zeta)
\]$.

Its dependence on $\(x\)$ describes variation across emergent spacetime, while its dependence on $\(\zeta\)$ encodes the internal informational structure that is invisible in the coarse-grained spacetime description.


---

2. The entropic distribution on each fiber

Obidi introduces an entropic distribution

$\[
f_{\mathrm{ent}}(x,\Pi,\zeta)
\]$.

where $\(\Pi_\mu\)$ is the generalized four-momentum associated with an entropic excitation.

The variables $\(\Pi_\mu\)$ need not initially be interpreted as ordinary particle momentum. They represent the spacetime-directed transport of entropic-information content. In the low-energy Lorentzian limit, they are identified with physical four-momentum.

The invariant integration measure on the fiber is denoted by

$\[
d\Omega_x(\Pi,\zeta)
\]$.

Thus, each spacetime event $\(x\)$ contains an entire fiber of microscopic entropic states.


---

3. Zeroth, first, and second fiber moments

The key construction follows the moment hierarchy used in kinetic theory.

Zeroth moment: entropic density

$\[
n_{\mathrm{ent}}(x)
=\int_{\mathcal F_x}
f_{\mathrm{ent}}(x,\Pi,\zeta)\,
d\Omega_x
\]$.

This gives a scalar density. It can represent the concentration or number density of entropic excitations.

First moment: entropic current

$\[
J_{\mu}^{(\mathrm{ent})}(x)
=\int_{\mathcal F_x}
\Pi_\mu
f_{\mathrm{ent}}(x,\Pi,\zeta)\,
d\Omega_x
\]$.

This gives a spacetime current describing the directed flow of entropic content.

Second moment: entropic stress-energy tensor

The decisive step is the second moment:

$\[
\boxed{
T_{\mu\nu}^{(\mathrm{ent})}(x)=
\int_{\mathcal F_x}
\Pi_\mu\Pi_\nu\,
f_{\mathrm{ent}}(x,\Pi,\zeta)\,
d\Omega_x
}
\]$

or, more generally,

$\[
\boxed{
T_{\mu\nu}^{(\mathrm{ent})}(x)
=\int_{\mathcal F_x}
\tau_{\mu\nu}(x,\Pi,\zeta)\,
d\Omega_x,
}
\]$

where $\(\tau_{\mu\nu}\)$ is the microscopic entropic stress kernel.

This is the central fiber-integral construction.

The tensorial character does not come from the integration itself. It comes from the rank-two object

$\[
\Pi_\mu\Pi_\nu
\]$

or from the more general microscopic tensor $\(\tau_{\mu\nu}\)$. Fiber integration removes the internal variables while preserving the spacetime indices $\(\mu,\nu\)$.

In differential-geometric language, this is the pushforward

$\[
T_{\mu\nu}^{(\mathrm{ent})}
=\pi_!\left(
\tau_{\mu\nu}\,d\Omega
\right)
\]$.

where $\(\pi_!\)$ denotes integration along the fibers.


---

4. Why the second moment becomes stress-energy

The components of the fiber-integrated tensor have the same physical interpretation as the components of the ordinary stress-energy tensor.

In a local Lorentz frame,

$\[
T_{00}^{(\mathrm{ent})}
=\int_{\mathcal F_x}
\Pi_0\Pi_0 f_{\mathrm{ent}}\,d\Omega_x
\]$

represents entropic energy density.

The mixed components

$\[
T_{0i}^{(\mathrm{ent})}
=\int_{\mathcal F_x}
\Pi_0\Pi_i f_{\mathrm{ent}}\,d\Omega_x
\]$

represent energy flux or momentum density.

The spatial components

$\[
T_{ij}^{(\mathrm{ent})}
=\int_{\mathcal F_x}
\Pi_i\Pi_j f_{\mathrm{ent}}\,d\Omega_x
\]$

represent pressure, momentum flux, shear stress, and anisotropic stress.

Thus the usual physical quantities on the right-hand side of Einstein’s equations arise as different projections of one fiber-integrated entropic tensor:

$\[
\begin{aligned}
\text{energy density}
&\longleftrightarrow T_{00}^{(\mathrm{ent})},\\
\text{momentum density}
&\longleftrightarrow T_{0i}^{(\mathrm{ent})},\\
\text{pressure}
&\longleftrightarrow \frac{1}{3}h^{ij}T_{ij}^{(\mathrm{ent})},\\
\text{shear stress}
&\longleftrightarrow
T_{\langle ij\rangle}^{(\mathrm{ent})}.
\end{aligned}
\]$

In Obidi’s physical interpretation:

$\[
\boxed{
\text{matter is a stable or condensed organization of the Entropic Field}
}
\]$

and

$\[
\boxed{
\text{radiation is a propagating excitation of the Entropic Field}
}
\]$.

Consequently, mass density, energy density, momentum, pressure, radiation flux, and stress are different coarse-grained moments of the underlying entropic distribution.


---

5. The field-theoretic form of the same construction

The kinetic expression can also be obtained from an action.

Suppose the microscopic entropic field on the bundle has a Lagrangian density

$\[
\mathcal L_{\mathrm{ent}}
=\mathcal L_{\mathrm{ent}}
\left(
S,D_AS,g_{\mu\nu},h_{ab},\zeta
\right)
\]$.

where:

$\(D_A\)$ denotes derivatives on the total bundle;

$\(g_{\mu\nu}\)$ is the emergent base metric;

$\(h_{ab}\)$ is a possible metric on the fibers.


The entropic action can be written as

$\[
I_{\mathrm{ent}}
=\int_{\mathcal M}
d^4x\,\sqrt{-g}
\int_{\mathcal F_x}
\mathcal L_{\mathrm{ent}}(x,\zeta)\,
d\mu_{\mathcal F_x}.
\]$

Define the effective spacetime Lagrangian by fiber integration:

$\[
\mathcal L_{\mathrm{eff}}(x)
=\int_{\mathcal F_x}
\mathcal L_{\mathrm{ent}}(x,\zeta)\,
d\mu_{\mathcal F_x}
\]$.

Then

$\[
I_{\mathrm{ent}}
=\int_{\mathcal M}
d^4x\,\sqrt{-g}\,
\mathcal L_{\mathrm{eff}}.
\]$

The effective entropic stress-energy tensor is defined by metric variation:

$\[
\boxed{
T_{\mu\nu}^{(\mathrm{ent})}
=-\frac{2}{\sqrt{-g}}
\frac{\delta I_{\mathrm{ent}}}
{\delta g^{\mu\nu}}.
}
\]$

Under minimal coupling, and provided the variation may be passed through the fiber integral,

$\[
T_{\mu\nu}^{(\mathrm{ent})}(x)
=\int_{\mathcal F_x}
\tau_{\mu\nu}^{(\mathrm{ent})}(x,\zeta)\,
d\mu_{\mathcal F_x},
\]$

where

$\[
\tau_{\mu\nu}^{(\mathrm{ent})}(x,\zeta)
=-\frac{2}{\sqrt{-g}}
\frac{\delta\left[
\sqrt{-g}\mathcal L_{\mathrm{ent}}(x,\zeta)
\right]}
{\delta g^{\mu\nu}}
\]$.

This shows that the fiber-moment construction and the action-variation construction are two formulations of the same mechanism.


---

6. Example for a scalar Entropic Field

For a minimally coupled scalar entropic field, one may take

$\[
\mathcal L_{\mathrm{ent}}
=-\frac{1}{2}
Z(S,\zeta)
g^{\alpha\beta}
D_\alpha S D_\beta S-
V(S,\zeta).
\]$

The microscopic entropic stress kernel is then

$\[
\tau_{\mu\nu}^{(\mathrm{ent})}=
Z(S,\zeta)
D_\mu S D_\nu S-
g_{\mu\nu}
\left[
\frac{1}{2}
Z(S,\zeta)
D_\alpha S D^\alpha S+
V(S,\zeta)\right]
\]$.

Fiber integration gives

$\[
\boxed{T_{\mu\nu}^{(\mathrm{ent})}(x)=\int_{\mathcal F_x}\left\{Z(S,\zeta)D_\mu S D_\nu S-g_{\mu\nu}\left[\frac{1}{2}Z(S,\zeta)D_\alpha S D^\alpha S+V(S,\zeta)\right]
\right\}d\mu_{\mathcal F_x}.}
\]$

The gradient term contributes directed energy and momentum flux, while the potential term contributes an isotropic energy density and pressure-like component.


---

7. Coupling to the emergent gravitational sector

The total effective action is written schematically as

$\[
I_{\mathrm{total}}=
I_{\mathrm{geometry}}+
I_{\mathrm{ent}}.
\]$

In the Lorentzian, near-equilibrium sector, the geometric part reduces to the Einstein–Hilbert form:

$\[
I_{\mathrm{geometry}}
=\frac{c^4}{16\pi G}\int_{\mathcal M}d^4x\,\sqrt{-g}\left(R-2\Lambda\right)
\]$.

Therefore,

$\[
I_{\mathrm{total}}
=\frac{c^4}{16\pi G}\int_{\mathcal M}
d^4x\,\sqrt{-g}\left(R-2\Lambda\right)+
I_{\mathrm{ent}}.
\]$

Variation of the geometric part gives

$\[
\delta I_{\mathrm{geometry}}=
\frac{c^4}{16\pi G}
\int_{\mathcal M}
d^4x\,\sqrt{-g}\left(G_{\mu\nu}+\Lambda g_{\mu\nu}\right)\delta g^{\mu\nu}.
\]$

Variation of the entropic part gives

$\[
\delta I_{\mathrm{ent}}=-\frac{1}{2}
\int_{\mathcal M}
d^4x\,\sqrt{-g}\,
T_{\mu\nu}^{(\mathrm{ent})}
\delta g^{\mu\nu}.
\]$

Stationarity,

$\[
\delta I_{\mathrm{total}}=0,
\]$

then requires

$\[
\frac{c^4}{16\pi G}
\left(G_{\mu\nu}+
\Lambda g_{\mu\nu}\right)-\frac{1}{2}T_{\mu\nu}^{(\mathrm{ent})}=0.
\]$

Multiplying by \(16\pi G/c^4\) gives

$\[
\boxed{
G_{\mu\nu}+
\Lambda g_{\mu\nu}=
\frac{8\pi G}{c^4}
T_{\mu\nu}^{(\mathrm{ent})}.}
\]$

Thus the right-hand side is

$\[
\boxed{
\frac{8\pi G}{c^4}
T_{\mu\nu}^{(\mathrm{ent})}=
\frac{8\pi G}{c^4}
\int_{\mathcal F_x}
\tau_{\mu\nu}^{(\mathrm{ent})}
\,d\mu_{\mathcal F_x}}
\]$.

In the kinetic representation,

$\[
\boxed{
G_{\mu\nu}+
\Lambda g_{\mu\nu}=
\frac{8\pi G}{c^4}
\int_{\mathcal F_x}
\Pi_\mu\Pi_\nu
f_{\mathrm{ent}}(x,\Pi,\zeta)
\,d\Omega_x}
\]$.

This is the compact form of Obidi’s fiber-integral derivation of the Einstein source term.


---

8. Recovery of ordinary matter

Obidi then takes the low-energy, near-equilibrium, Lorentzian-sector limit:

$\[
T_{\mu\nu}^{(\mathrm{Einstein})}
=\lim_{\substack{
\mathrm{IR}\\
\nabla S\rightarrow 0\\
\text{quantum corrections}\rightarrow 0
}}T_{\mu\nu}^{(\mathrm{ent})}.
\]$

Equivalently,

$\[
\boxed{
T_{\mu\nu}^{(\mathrm{matter})}=
\lim_{\mathrm{IR}}
\int_{\mathcal F_x}
\Pi_\mu\Pi_\nu
f_{\mathrm{ent}}(x,\Pi,\zeta)
\,d\Omega_x.
}
\]$

Within the sector decomposition previously used in the Obidi framework,

$\[
T_{(\mu\nu)_J}^{(\mathrm{ent})}
=T_{(\mu\nu)_{\mathrm{FR}}}^{(\mathrm{ent})}+
T_{(\mu\nu)_{\mathrm{FS}}}^{(\mathrm{ent})}+
T_{(\mu\nu)_{\mathrm L}}^{(\mathrm{ent})}.
\]$

Here:

the Fisher–Rao sector carries classical statistical-information contributions;

the Fubini–Study sector carries quantum-state contributions;

the Lorentzian sector carries the effective physical spacetime source.


In the classical near-equilibrium limit,

$\[T_{(\mu\nu)_{\mathrm L}}^{(\mathrm{ent})}
\longrightarrowT_{\mu\nu}^{(\mathrm{matter})},
\]$

while the Fisher–Rao and Fubini–Study corrections become negligible or are absorbed into effective couplings.


---

9. Perfect-fluid limit

For an isotropic distribution of entropic excitations in a local rest frame, the second fiber moment reduces to the perfect-fluid form

$\[
\boxed{
T_{\mu\nu}^{(\mathrm{ent})}=
\frac{\varepsilon+p}{c^2}u_\mu u_\nu+
p\,g_{\mu\nu}}
\]$,

where

$\[
\varepsilon
=\int_{\mathcal F_x}
E^2 f_{\mathrm{ent}}\,d\Omega_x
\]$

is the effective energy density and

$\[p=
\frac{1}{3}
\int_{\mathcal F_x}
|\boldsymbol{\Pi}|^2
f_{\mathrm{ent}}\,d\Omega_x
\]$

is the isotropic pressure, up to the normalization conventions of the invariant fiber measure.

This shows how the familiar matter source of cosmology and relativistic fluid mechanics can emerge from an underlying entropic distribution.


---

10. Conservation of the fiber-integrated tensor

Einstein’s tensor satisfies the contracted Bianchi identity:

$\[
\nabla^\mu G_{\mu\nu}=0.
\]$

Therefore the entropic source must satisfy

$\[
\nabla^\mu T_{\mu\nu}^{(\mathrm{ent})}=0.
\]$

In Obidi’s construction, this conservation can arise in either of two equivalent ways.

First, it follows from diffeomorphism invariance of the fiber-integrated entropic action.

Second, in the kinetic formulation, it follows by taking a momentum moment of an entropic transport equation,

$\[
\Pi^A D_A f_{\mathrm{ent}}=
C[f_{\mathrm{ent}}]
\]$,

provided the interaction term conserves generalized entropic four-momentum:

$\[
\int_{\mathcal F_x}
\Pi_\nu C[f_{\mathrm{ent}}]
\,d\Omega_x=0
\]$.

Then

$\[
\nabla^\mu
\int_{\mathcal F_x}
\Pi_\mu\Pi_\nu f_{\mathrm{ent}}
\,d\Omega_x=0
\]$.

Hence,

$\[
\nabla^\mu T_{\mu\nu}^{(\mathrm{ent})}=0.
\]$


---

11. What the fiber integral does—and does not—derive

The fiber integral explains how a microscopic Entropic Field can generate the tensorial structure of the Einstein source:

$\[
\text{internal entropic degrees of freedom}\quad\stackrel{\pi_!}{\longrightarrow}\quad T_{\mu\nu}
\]$.

However, the numerical gravitational coupling

$\[
\frac{8\pi G}{c^4}
\]$

does not follow from the fiber integral alone. It enters through the relative normalization of the emergent geometric action and the entropic action. To claim a complete first-principles derivation, ToE must derive that normalization from the microscopic entropic parameters rather than merely match it to the Einstein–Hilbert limit.

Likewise, a fully completed theory must specify:

$\[
\mathcal F_x,\qquad
d\Omega_x,\qquad
f_{\mathrm{ent}},\qquad
\Pi_\mu,\qquad
\mathcal L_{\mathrm{ent}},
\]$

and demonstrate how known matter fields, particle masses, gauge charges, equations of state, and interaction couplings arise from them.

Summary statement

Obidi derived the right-hand side of Einstein’s field equations by treating ordinary matter-energy as the spacetime projection of microscopic entropic-information degrees of freedom. He formed a rank-two microscopic stress kernel—most directly $\(\Pi_\mu\Pi_\nu f_{\mathrm{ent}}\)$—and pushed it forward from the entropic fiber bundle to spacetime:

$\[
T_{\mu\nu}^{(\mathrm{ent})}(x)=\pi_!
\left(
\Pi_\mu\Pi_\nu f_{\mathrm{ent}}\,d\Omega
\right)=
\int_{\mathcal F_x}
\Pi_\mu\Pi_\nu
f_{\mathrm{ent}}
\,d\Omega_x.
\]$

Metric variation of the fiber-integrated Obidi Action then produces

$\[
G_{\mu\nu}+
\Lambda g_{\mu\nu}=
\frac{8\pi G}{c^4}
T_{\mu\nu}^{(\mathrm{ent})}
\]$.

In the infrared, near-equilibrium Lorentzian limit,

$\[
T_{\mu\nu}^{(\mathrm{ent})}
\longrightarrow
T_{\mu\nu}^{(\mathrm{matter})}
\]$,

so the conventional right-hand side of Einstein’s equations appears as the coarse-grained second fiber moment of the fundamental Entropic Field.
