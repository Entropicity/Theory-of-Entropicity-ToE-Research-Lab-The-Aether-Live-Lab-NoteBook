# DRAFT: WORK IN PROGRESS, UNDER CONSTRUCTION

# From Entropy to the Obidi Action: DRAFT

## A Step-by-Step Variational Derivation of the Obidi Action of the Theory of Entropicity (ToE)

**Framework:** John Onimisi Obidi’s Theory of Entropicity (ToE)  
**Document type:** Explanatory theoretical paper and mathematical derivation  
**Scope:** Entropy, information geometry, entropic field dynamics, the Principle of Least Entropic Resistance, and the Haller–Obidi correspondence

## Abstract

The Theory of Entropicity (ToE) proposes that entropy-related structure has a primary physical role and that dynamics should be formulated in terms of an entropic substrate. This paper reconstructs a mathematically consistent route from that proposal to an Obidi action. It distinguishes statistical definitions, ontological postulates, geometric prescriptions, and consequences of variational calculus. Beginning with probability distributions, entropy, and relative surprisal, the discussion explains how information geometry supplies a measure of statistical distinguishability while identifying the additional structure needed for a nondegenerate Lorentzian metric. Locality, covariance, a two-derivative truncation, and positive kinetic energy then motivate a minimal scalar-field action. Its dimensions, signs, boundary conditions, Euler–Lagrange equation, and stress tensor are derived explicitly. A scalar–tensor completion incorporates genuine curvature and permits independent metric dynamics. A separate path variation gives a precise formulation of the Principle of Least Entropic Resistance. The Haller–Obidi relation is examined as an entropy–action identity, with particular attention to the difference between accumulated path-dependent entropy and the total derivative of a local scalar. Conservation, entropy production, finite propagation speed, localization, and quantum extensions are addressed with their assumptions stated. The resulting account explains the logical construction of an entropic action without treating the postulates required for that construction as consequences of Shannon entropy alone.

**Keywords:** Theory of Entropicity; Obidi action; entropic field; Fisher information; Lorentzian geometry; variational principle; scalar–tensor theory; entropic resistance; Haller–Obidi correspondence.

## Editorial and source statement

This paper is a technically checked reconstruction of the framework supplied for discussion. It is not a historical verification of every step in Obidi’s manuscripts, a claim of experimental confirmation, or a proof that the action is uniquely implied by information theory. Obidi’s Letter IB explicitly presents the Haller–Obidi identity and claims a localization correspondence [1]. The abstract available for the preceding analysis did not contain the full localization calculation; that proof is therefore not certified here. Haller’s conference paper supplies the earlier entropy–action context [2].

The body reorganizes and expands the preceding explanation into a paper. **Appendix A preserves that explanation in full**, including all fifty numbered equations, the unnumbered expressions, the notation table, the logical qualifications, and its concluding formulation. Mathematical delimiters have been changed to GitHub-compatible inline and display forms. Chat-specific citation markers have been replaced with numbered references. This preserves the source material while allowing the paper itself to use a professional structure.

## 1. The logical question: what does it mean to arrive at an action?

An action is a functional: it assigns a number to an entire field configuration or history. Its stationary configurations define candidate physical evolutions once the allowed variations and boundary conditions have been specified.

The reasoning examined here contains four distinct operations:

1. **Definition:** construct entropy-related quantities from probability distributions.
2. **Physical postulate:** assign an entropy-related field an ontological and causal role.
3. **Model construction:** specify geometry, locality, symmetries, derivative order, and couplings.
4. **Derivation:** vary the resulting action and calculate its consequences.

These operations are complementary. Making their boundaries explicit strengthens the proposal because it identifies what follows mathematically and what constitutes the theory’s physical input.

Obidi’s central move, as represented in the supplied framework, is the promotion of an entropy-related quantity into a field with physical significance. The action is then constructed to govern this field. In that sense, the route is a derivation of field equations from an entropy-first model, with the model’s assumptions stated. It is not a unique derivation of all dynamics from the Shannon functional alone.

## 2. Notation, units, and mathematical setting

Entropy and action must not be represented by an undifferentiated use of the same symbol.

| Symbol | Meaning | Units or role |
|---|---|---|
| $H$ | Information entropy | Dimensionless, in nats |
| $S_{\mathrm{ent}}$ | Entropy with physical units | Energy/temperature |
| $s=S_{\mathrm{ent}}/k_B$ | Normalized entropic scalar | Dimensionless |
| $\lambda$ | Relative surprisal | Dimensionless |
| $\Lambda$ | Entropy-scaled logarithmic probability field | Energy/temperature |
| $\mathcal A_{\mathrm O}$ | Obidi action | Energy × time |
| $M$ | Differentiable manifold | Base manifold of the effective theory |
| $x^\mu$ | Coordinates on $M$ | Length when $x^0=ct$ |
| $y$ | Microstate variable | Distinct from $x^\mu$ |
| $\theta^a$ | Statistical model parameters | Coordinates on a statistical manifold |
| $G_{ab}$ | Fisher information metric | Statistical distinguishability |
| $h_{\mu\nu}$ | Positive-definite metric when nondegenerate | Information or resistance geometry |
| $g_{\mu\nu}$ | Lorentzian metric | Signature $(-,+,+,+)$ |
| $\kappa$ | Constant scalar kinetic coefficient | Energy/length |
| $K(s)$ | Field-dependent kinetic coefficient | Energy/length |
| $U(s)$ | Potential-energy density | Energy/volume |
| $F(s)$ | Curvature-coupling coefficient | Energy/length |

We use a Levi-Civita connection for the spacetime metric, unless a different connection is explicitly indicated. For a scalar,

$$
\nabla_\mu s=\partial_\mu s.
$$

The manifold is taken to be four-dimensional in the effective relativistic formulation. Choosing four dimensions is an assumption of this construction; the existence of four physical dimensions has not been derived from an entropy definition.

## 3. From probability to entropy and surprisal

### 3.1 Discrete entropy

For a normalized distribution,

$$
p_i\geq0,
\qquad
\sum_i p_i=1,
$$

Shannon entropy is

$$
H[p]=-\sum_i p_i\ln p_i,
\qquad
S_{\mathrm{ent}}[p]=k_BH[p].
$$

The natural logarithm gives entropy in nats. The conventional limiting definition makes the contribution $p_i\ln p_i$ vanish when $p_i=0$.

The individual quantity $-\ln p_i$ is surprisal. Entropy is its probability-weighted mean. This distinction matters when a logarithmic quantity is promoted to a field: the local quantity and its ensemble average generally retain different information.

### 3.2 Continuous distributions and the reference density

A probability density depends on the measure relative to which it is defined. Writing the logarithm of a dimensional density without specifying a reference can create a units problem. A clean construction uses densities $p(y)$ and $q(y)>0$ relative to the same measure:

$$
\int p(y)\,d\mu(y)=1,
\qquad
H_q[p]=-\int p(y)\ln\!\left(\frac{p(y)}{q(y)}\right)d\mu(y).
$$

When both densities are normalized, this is

$$
H_q[p]=-D_{\mathrm{KL}}(p\Vert q).
$$

It is then nonpositive and should be called a relative-entropy-based quantity rather than ordinary thermodynamic entropy. A signed scalar can still be used as a field variable; its sign does not invalidate the field theory. The physical interpretation must match the definition.

The ratio is unchanged by a simultaneous change of microstate coordinates because the same density Jacobian occurs in numerator and denominator. This is the relevant coordinate-invariance property.

### 3.3 Local distributions

Associate a probability distribution with each point of the base manifold:

$$
p(y\mid x),
\qquad
\int p(y\mid x)\,d\mu(y)=1.
$$

One possible scalar is

$$
s(x)
=-\int p(y\mid x)
\ln\!\left(\frac{p(y\mid x)}{q(y)}\right)d\mu(y).
$$

The corresponding relative surprisal is

$$
\lambda(y,x)
=-\ln\!\left(\frac{p(y\mid x)}{q(y)}\right),
\qquad
s(x)=\int p(y\mid x)\lambda(y,x)\,d\mu(y).
$$

The microstate label $y$ and the manifold coordinate $x$ have separate roles. The first expression averages over microstates at a fixed manifold point.

Alternatively, a promoted logarithmic probability field may be defined by

$$
\Lambda(x)
=-k_B\ln\!\left(\frac{p(x)}{p_*(x)}\right).
$$

Here $p$ and $p_*$ must be comparable densities or probabilities so that their ratio is dimensionless and transforms as a scalar. This expression is not automatically the averaged entropy field above.

### 3.4 The ontological step

The construction of a scalar from probabilities is mathematical. Declaring that scalar to be a primary causal substrate is the ToE postulate. Once that postulate is adopted, the next task is to specify its dynamics.

A further modeling decision arises if $s$ is retained as a composite function of probabilities. Varying $s$ as an unrestricted independent field need not be equivalent to varying the underlying probabilities subject to normalization. The scalar action below is most directly understood as an effective description in which $s$ is an independent variable. A microscopic derivation must explain how that effective description is obtained.

## 4. How probability supplies information geometry

### 4.1 Derivation of the local metric

For a regular family $p(y\mid\theta)$, define the score

$$
u_a(y,\theta)=\partial_a\ln p(y\mid\theta).
$$

Differentiating normalization, assuming differentiation and integration may be interchanged, gives

$$
\int p\,u_a\,d\mu=0.
$$

Differentiating once more yields

$$
0
=\int p
\left(
u_au_b+\partial_a\partial_b\ln p
\right)d\mu.
$$

Therefore

$$
G_{ab}
=\int p\,u_au_b\,d\mu
=-\int p\,\partial_a\partial_b\ln p\,d\mu.
$$

Expanding the relative entropy between neighboring distributions gives

$$
\begin{aligned}
D_{\mathrm{KL}}(p_\theta\Vert p_{\theta+d\theta})
&=\int p_\theta
\left[
\ln p_\theta-\ln p_{\theta+d\theta}
\right]d\mu\\
&=-\left\langle u_a\right\rangle d\theta^a
-\frac12
\left\langle\partial_a\partial_b\ln p\right\rangle
d\theta^a d\theta^b
+O(\|d\theta\|^3)\\
&=\frac12G_{ab}\,d\theta^a d\theta^b
+O(\|d\theta\|^3).
\end{aligned}
$$

The vanishing linear term and the quadratic leading term explain why distinguishability defines a metric locally. The geometric framework is discussed in Nielsen [3].

For any vector $v^a$,

$$
v^aG_{ab}v^b
=\int p\left(v^au_a\right)^2d\mu\geq0.
$$

This proves positive semidefiniteness directly. Positive definiteness requires that no nonzero parameter direction leave the distribution unchanged to first order.

### 4.2 When a Hessian is a Fisher metric

For an exponential family,

$$
p(y\mid\theta)
=h(y)\exp\!\left[\theta^aT_a(y)-\psi(\theta)\right],
$$

normalization implies

$$
\partial_a\psi=\langle T_a\rangle,
\qquad
\partial_a\partial_b\psi
=\operatorname{Cov}(T_a,T_b)=G_{ab}.
$$

The Hessian formula is valid in these natural coordinates. It does not justify identifying an arbitrary ordinary Hessian of mutual information with a spacetime metric. Under general nonlinear coordinate transformations, an ordinary Hessian of a scalar acquires additional terms and is not automatically a tensor.

### 4.3 Pullback and the rank obstruction

If statistical parameters are functions of manifold coordinates, their Fisher metric pulls back to

$$
h_{\mu\nu}
=G_{ab}(\theta(x))
\partial_\mu\theta^a\partial_\nu\theta^b.
$$

If $\theta^a=\theta^a(s)$, the chain rule gives

$$
h_{\mu\nu}
=
\left[
G_{ab}\frac{d\theta^a}{ds}\frac{d\theta^b}{ds}
\right]\partial_\mu s\partial_\nu s
=C(s)\partial_\mu s\partial_\nu s.
$$

This tensor has rank at most one. A nondegenerate four-dimensional metric therefore cannot be obtained from that particular one-parameter pullback. This is a limitation of the specified construction, not a proof that every possible scalar-based geometric model is impossible. A viable model must state what additional structure supplies the remaining independent directions.

## 5. From positive information geometry to Lorentzian geometry

Positive-definite Fisher geometry cannot become Lorentzian merely through a real invertible coordinate transformation: such a transformation preserves the numbers of positive and negative metric directions.

A possible additional prescription is

$$
h^{\mu\nu}n_\mu n_\nu=1,
\qquad
g_{\mu\nu}=h_{\mu\nu}-2n_\mu n_\nu.
$$

In an orthonormal frame aligned with the unit covector,

$$
h_{\mu\nu}=\operatorname{diag}(1,1,1,1),
\qquad
g_{\mu\nu}=\operatorname{diag}(-1,1,1,1).
$$

The prescription reverses the sign of one metric direction. To use it as a realization of an Obidi transformation, the theory must determine the direction $n_\mu$, its dynamics or constraints, and its behavior where a proposed defining quantity vanishes. A globally defined unit direction is also an additional global assumption.

For example, a nonvanishing gradient could select a local direction through

$$
n_\mu
=\frac{\partial_\mu s}
{\sqrt{h^{\alpha\beta}\partial_\alpha s\partial_\beta s}}.
$$

This example fails where the gradient vanishes and presupposes an already nondegenerate $h_{\mu\nu}$. It is illustrative, not an established equation attributed to Obidi.

The replacement defines a causal signature. It does not, by itself, derive a thermodynamic arrow, quantum theory, or a numerical propagation speed.

## 6. Constructing the minimal Obidi action

### 6.1 Invariant integration

Let $g=\det(g_{\mu\nu})$. With Lorentzian signature and $x^0=ct$, the action is

$$
\mathcal A_{\mathrm O}
=\frac1c\int_M\sqrt{-g}\,
\mathcal L_{\mathrm O}\,d^4x.
$$

Under a coordinate change, the determinant factor and coordinate volume acquire inverse Jacobian factors, so their product is invariant. The scalar $\mathcal L_{\mathrm O}$ has units of energy density; $\sqrt{-g}\mathcal L_{\mathrm O}$ is the corresponding coordinate density.

### 6.2 Physical and mathematical assumptions

The minimal construction assumes a real scalar field, locality, coordinate invariance, a truncation to terms containing at most two derivatives in total, and a positive kinetic coefficient. At this order the simplest derivative scalar is

$$
X=g^{\mu\nu}\nabla_\mu s\nabla_\nu s.
$$

A term linear in $\Box_gs$ with a field-dependent coefficient can be reduced by integration by parts to a kinetic term plus a boundary term. Higher powers such as $X^2$ lie beyond the stated two-derivative truncation, even though some such models can still have second-order field equations. Derivative counting and differential-equation order should therefore not be confused.

The resulting minimal choice is

$$
\boxed{
\mathcal A_{\mathrm O}^{\mathrm{min}}[s;g]
=\frac1c\int_M\sqrt{-g}
\left[
-\frac{\kappa}{2}
g^{\mu\nu}\nabla_\mu s\nabla_\nu s
-U(s)
\right]d^4x,
\qquad \kappa>0.
}
$$

The semicolon indicates that the metric is initially treated as a specified background. Geometry becomes dynamical only when an appropriate metric sector is supplied and varied.

The term involving $\kappa$ penalizes spatial inhomogeneity in the energy and supplies inertia for temporal variation. The potential specifies local preferences, equilibria, and restoring forces. Neither is fixed numerically by Shannon entropy.

### 6.3 Dimensional and energy checks

Since $s$ is dimensionless,

$$
[\nabla_\mu s]=\mathrm{length}^{-1},
\qquad
[\kappa]=\frac{\mathrm{energy}}{\mathrm{length}},
\qquad
[U]=\frac{\mathrm{energy}}{\mathrm{length}^3}.
$$

The integral has units of energy × time. A bare coefficient $\hbar^2$ or $\hbar/2$ cannot replace $\kappa$ under these conventions without additional scales or field normalization.

In flat spacetime,

$$
\mathcal L_{\mathrm O}
=\frac{\kappa}{2c^2}\dot s^{\,2}
-\frac{\kappa}{2}|\boldsymbol\nabla s|^2-U(s).
$$

The canonical momentum density and Hamiltonian density are

$$
\pi=\frac{\partial\mathcal L_{\mathrm O}}{\partial\dot s}
=\frac{\kappa}{c^2}\dot s,
$$

$$
\mathcal H
=\pi\dot s-\mathcal L_{\mathrm O}
=\frac{\kappa}{2c^2}\dot s^{\,2}
+\frac{\kappa}{2}|\boldsymbol\nabla s|^2+U(s).
$$

Thus $\kappa>0$ supplies positive kinetic and gradient energies. A suitable lower bound on $U$ is also needed for a globally bounded energy. Positivity of the kinetic coefficient alone does not establish every form of stability.

## 7. Field variation, with every calculus step shown

Hold the metric fixed and vary $s$ by $s+\epsilon\delta s$. Because the two gradient factors give equal contributions,

$$
\delta\!\left[
-\frac{\kappa}{2}
g^{\mu\nu}\nabla_\mu s\nabla_\nu s
\right]
=-\kappa\nabla^\mu s\nabla_\mu\delta s.
$$

Also,

$$
\delta U(s)=U'(s)\delta s.
$$

Therefore

$$
\delta\mathcal A_{\mathrm O}^{\mathrm{min}}
=\frac1c\int_M\sqrt{-g}
\left[
-\kappa\nabla^\mu s\nabla_\mu\delta s
-U'(s)\delta s
\right]d^4x.
$$

Use the identity

$$
\nabla_\mu(\delta s\,\nabla^\mu s)
=\nabla_\mu\delta s\,\nabla^\mu s
+\delta s\,\Box_gs,
$$

where

$$
\Box_gs
=\frac1{\sqrt{-g}}
\partial_\mu
\left(\sqrt{-g}\,g^{\mu\nu}\partial_\nu s\right).
$$

Integration by parts transfers the derivative from the arbitrary variation to the field. Compactly supported variations, or fixed field values at a suitable boundary, remove the surface contribution. The result is

$$
\delta\mathcal A_{\mathrm O}^{\mathrm{min}}
=\frac1c\int_M\sqrt{-g}
\left[\kappa\Box_gs-U'(s)\right]\delta s\,d^4x.
$$

Since the interior variation is arbitrary,

$$
\boxed{\kappa\Box_gs-U'(s)=0.}
$$

This is the field equation derived from the chosen action. The variational method is standard [4]; the proposed entropic meaning of the field is the ToE interpretation.

For a quadratic potential,

$$
U(s)=\frac{\kappa\mu^2}{2}s^2,
$$

the equation becomes

$$
\frac1{c^2}\partial_t^2s-\nabla^2s+\mu^2s=0.
$$

A plane-wave substitution gives

$$
\omega^2=c^2\left(|\mathbf k|^2+\mu^2\right),
$$

which checks the mass-term sign. More generally, an equilibrium $s_0$ with $U'(s_0)=0$ has a nonnegative linearized mass squared when $U''(s_0)/\kappa\geq0$.

If $\kappa$ is replaced by $K(s)$, the derivative of the coefficient also contributes:

$$
\nabla_\mu(K\nabla^\mu s)
-\frac12K'(\nabla s)^2-U'=0,
$$

or

$$
\boxed{
K\Box_gs+\frac12K'(\nabla s)^2-U'=0.
}
$$

## 8. Genuine curvature and a scalar–tensor completion

A squared gradient is a kinetic invariant. Curvature instead measures the geometric variation of parallel transport and is encoded by tensors constructed from the connection and metric. To make curvature explicit, one possible completion is

$$
\boxed{
\mathcal A_{\mathrm O}
=\frac1c\int_M\sqrt{-g}
\left[
\frac12F(s)R[g]
-\frac12K(s)(\nabla s)^2-U(s)
\right]d^4x
+\mathcal A_{\mathrm m}
+\mathcal A_{\partial M}.
}
$$

This is a possible scalar–tensor model, not a unique consequence of the entropy postulate. Boundary terms must be chosen consistently with the class of boundary, the varied fields, and the fixed boundary data. Null boundaries can require different treatment from non-null boundaries.

Assuming that the matter action has no explicit $s$ dependence, the scalar equation is

$$
K\Box_gs+\frac12K'(\nabla s)^2+\frac12F'R-U'=0.
$$

Explicit scalar–matter coupling would add the corresponding matter variation and must not be omitted.

Define the stress tensor by varying the nongravitational action with respect to the inverse metric:

$$
T_{\mu\nu}
=-\frac{2c}{\sqrt{-g}}\,
\frac{\delta\mathcal A_{\mathrm{nongrav}}}{\delta g^{\mu\nu}}.
$$

The determinant variation is

$$
\delta\sqrt{-g}
=-\frac12\sqrt{-g}\,g_{\mu\nu}\delta g^{\mu\nu}.
$$

After the curvature boundary terms have been handled, independent metric variation gives

$$
F G_{\mu\nu}
=T_{\mu\nu}^{(s)}+T_{\mu\nu}^{(\mathrm m)}
+\nabla_\mu\nabla_\nu F-g_{\mu\nu}\Box_gF,
$$

where

$$
T_{\mu\nu}^{(s)}
=K\nabla_\mu s\nabla_\nu s
-g_{\mu\nu}
\left[\frac12K(\nabla s)^2+U\right].
$$

For constant

$$
F=\frac{c^4}{8\pi G},
$$

the action’s curvature coefficient is $c^3/(16\pi G)$ after the overall factor $1/c$ is included. The metric equation has Einstein normalization.

If instead $g_{\mu\nu}$ is defined from information variables, the correct variation must respect that definition. Schematically,

$$
\delta\mathcal A
=\int
\left[
\frac{\delta\mathcal A}{\delta s}\delta s
+\frac{\delta\mathcal A}{\delta g_{\mu\nu}}
\delta g_{\mu\nu}
\right],
$$

and $\delta g_{\mu\nu}$ contains variations of those underlying variables. Treating it as independent would change the theory unless constraints or an equivalent independent-field formulation are provided.

## 9. The Principle of Least Entropic Resistance

### 9.1 A path functional

A path principle varies trajectories. It is distinct from a field principle that varies configurations throughout a spacetime region.

Choose a positive-definite metric $h_{\mu\nu}$ and a resistance weight

$$
w(x)=h^{\mu\nu}\partial_\mu s\partial_\nu s.
$$

The proposed resistance functional is

$$
\mathcal R[\gamma]
=\int_\gamma w\,d\ell_h,
\qquad
d\ell_h^2=h_{\mu\nu}dx^\mu dx^\nu.
$$

Using a path parameter $\lambda$,

$$
L_\gamma
=w(x)q,
\qquad
q=\sqrt{h_{\mu\nu}\dot x^\mu\dot x^\nu}.
$$

The Euler–Lagrange equation is

$$
\frac{d}{d\lambda}
\left(\frac{\partial L_\gamma}{\partial\dot x^\mu}\right)
-\frac{\partial L_\gamma}{\partial x^\mu}=0.
$$

Its ingredients are

$$
\frac{\partial L_\gamma}{\partial\dot x^\mu}
=\frac{w h_{\mu\nu}\dot x^\nu}{q},
$$

$$
\frac{\partial L_\gamma}{\partial x^\mu}
=q\,\partial_\mu w
+\frac{w}{2q}
\partial_\mu h_{\alpha\beta}\dot x^\alpha\dot x^\beta.
$$

This explicit calculation corrects an attempted variation with respect to the field gradient when the intended variables are path coordinates.

### 9.2 Weighted geodesics

Choose arc length after deriving the parameter-invariant equation, and set

$$
T^\mu=\frac{dx^\mu}{d\ell_h},
\qquad
h_{\mu\nu}T^\mu T^\nu=1.
$$

The path equation becomes

$$
\nabla_T^{(h)}(wT_\mu)=\partial_\mu w.
$$

Expanding the derivative and raising the index gives

$$
\boxed{
w\,T^\nu\nabla_\nu^{(h)}T^\mu
=\left(h^{\mu\nu}-T^\mu T^\nu\right)\partial_\nu w.
}
$$

Only the component of the gradient perpendicular to the tangent changes the path’s direction.

Where $w>0$, define

$$
\widetilde h_{\mu\nu}=w^2h_{\mu\nu}.
$$

Then

$$
\sqrt{\widetilde h_{\mu\nu}dx^\mu dx^\nu}
=w\,d\ell_h.
$$

Thus the resistance functional is the length functional of a conformal metric. If the weight has units, a fixed reference weight may be inserted to make the conformal factor dimensionless; multiplication of the entire functional by a positive constant does not alter stationary paths.

The original gradient weight vanishes at critical points of the field. A possible regularization is

$$
w=w_0+\ell_*^2h^{\mu\nu}\partial_\mu s\partial_\nu s,
\qquad
w_0>0.
$$

This is a modified model, and its stationary paths need not coincide with those of the unregularized weight. It is not merely a change of notation.

Stationarity does not prove global minimization. Nor does this Riemannian resistance principle by itself produce timelike relativistic motion, a flux constitutive law, or the scalar-field action. Those connections need separate derivations.

## 10. The Haller–Obidi identity and its variational content

The relation reported in Letter IB is [1]

$$
H(t)-H(t_0)
=\frac2\hbar\int_{t_0}^{t}(mc^2-L)\,dt'.
$$

Differentiating,

$$
\frac{dH}{dt}=\frac2\hbar(mc^2-L),
$$

and rearranging,

$$
\boxed{
L_{\mathrm{HO}}
=mc^2-\frac{\hbar}{2}\frac{dH}{dt}.
}
$$

For entropy with physical units,

$$
L_{\mathrm{HO}}
=mc^2-\frac{\hbar}{2k_B}\frac{dS_{\mathrm{ent}}}{dt}.
$$

The coefficient is dimensionally correct because a dimensionless entropy rate multiplied by $\hbar$ has units of energy.

### 10.1 Local scalar entropy produces a boundary term

If $H(t)=s(x(t))$, then

$$
\frac{dH}{dt}=\partial_t s+\dot x^i\partial_i s,
$$

so

$$
\mathcal A_{\mathrm{HO}}
=mc^2(t_f-t_i)-\frac{\hbar}{2}(s_f-s_i).
$$

With fixed spacetime endpoints and constant mass, every term is fixed. The action supplies no bulk trajectory equation.

The cancellation can also be checked directly. For a smooth scalar,

$$
\frac{\partial L_{\mathrm{HO}}}{\partial\dot x^i}
=-\frac{\hbar}{2}\partial_i s,
$$

$$
\frac{d}{dt}
\frac{\partial L_{\mathrm{HO}}}{\partial\dot x^i}
=-\frac{\hbar}{2}
\left(\partial_t\partial_i s+\dot x^j\partial_j\partial_i s\right),
$$

which equals $\partial L_{\mathrm{HO}}/\partial x^i$ by equality of mixed partial derivatives.

### 10.2 Accumulated entropy can retain path dependence

If instead

$$
H[x](t)-H[x](t_0)
=\int_{t_0}^{t}r(x,\dot x,t')\,dt',
$$

and the integral cannot be expressed as a fixed local scalar difference, then the entropy contribution may affect the trajectory. Fixed coordinate endpoints do not generally fix such accumulated entropy.

The rate $r$ must be specified independently if the construction is to predict motion. Defining it afterward from a known Lagrangian reproduces an identity, but does not independently derive that Lagrangian.

### 10.3 Covariance requires consistent time parametrization

For proper time $\tau$,

$$
u^\mu=\frac{dx^\mu}{d\tau},
\qquad
u^\mu\nabla_\mu s=\frac{ds}{d\tau},
\qquad
\int u^\mu\nabla_\mu s\,d\tau=s_f-s_i.
$$

The entropy contribution remains a boundary term. The candidate expression

$$
L_{\mathrm{ent}}
=mc^2-\frac{\hbar}{2}u^\mu\nabla_\mu s
$$

must be interpreted together with its integration parameter and relativistic conventions. In an integral over proper time, the term $mc^2\int d\tau$ is path dependent, unlike the fixed coordinate-time constant in the preceding calculation. Its positive sign differs from the conventional free-particle action by an overall sign in the isolated free sector; relative signs matter when interactions are added.

Thus the coordinate-time and proper-time expressions cannot be interchanged without checking the complete action.

## 11. Localization and the classical limit

A field theory does not become a particle theory by merely evaluating its field along a curve. A localization argument must identify an appropriate concentrated solution or excitation and derive the dynamics of its collective coordinates.

A typical program is to construct a profile centered at $\mathbf X(t)$, substitute the profile into the field action, integrate over the internal spatial coordinates, and retain the leading terms in a controlled approximation. The result must establish an effective mass and the form of any interactions.

The target free relativistic action is

$$
\mathcal A_{\mathrm{pp}}=-mc^2\int d\tau.
$$

In flat spacetime,

$$
d\tau=dt\sqrt{1-\frac{v^2}{c^2}},
$$

and hence

$$
L_{\mathrm{pp}}
=-mc^2\sqrt{1-\frac{v^2}{c^2}}
=-mc^2+\frac12mv^2
+O\!\left(\frac{mv^4}{c^2}\right).
$$

The constant term may be dropped for fixed coordinate-time endpoints, leaving the Newtonian free-particle Lagrangian. An external potential requires a separately derived coupling.

A canonical real scalar with an arbitrary potential does not automatically admit stable localized particle-like solutions. Their existence, stability, and scale separation must be established in the chosen model. The schematic sequence from field action to Haller–Obidi action to classical mechanics therefore represents a correspondence to demonstrate, not a consequence of notation alone.

## 12. Stress-energy, Noether current, and thermodynamic entropy current

For the minimal field action,

$$
T_{\mu\nu}^{(s)}
=\kappa\nabla_\mu s\nabla_\nu s
-g_{\mu\nu}
\left[\frac{\kappa}{2}(\nabla s)^2+U(s)\right].
$$

Differentiate it covariantly. Metric compatibility and the equality of second covariant derivatives on a scalar cancel the mixed-gradient terms:

$$
\nabla^\mu T_{\mu\nu}^{(s)}
=\left(\kappa\Box_gs-U'\right)\nabla_\nu s.
$$

The field equation therefore implies on-shell conservation for the isolated minimally coupled scalar sector.

When $K=\kappa$ and $U$ is constant, a constant shift of $s$ is a symmetry. Up to an overall sign convention, its Noether current is

$$
J^\mu=\kappa\nabla^\mu s,
\qquad
\nabla_\mu J^\mu=0.
$$

For nonconstant $U$,

$$
\nabla_\mu J^\mu=U'(s).
$$

This current is not automatically a physical thermodynamic entropy flux. An entropy-current model might instead use

$$
J_S^\mu=\rho_Su^\mu,
\qquad
\nabla_\mu J_S^\mu=\sigma\geq0.
$$

Here $\rho_S$ is a rest-frame entropy density and $\sigma$ is entropy production. The convective form omits possible conductive or diffusive contributions, which would need to be included where physically relevant. Conservation is the special case $\sigma=0$.

For nonminimal curvature coupling, the scalar stress tensor as defined above need not be separately conserved. Its divergence includes the curvature-exchange contribution when $F'\neq0$. The full coupled equations, their Bianchi identity, and the matter assumptions determine the consistent balance law.

## 13. Finite propagation, irreversibility, and quantum extensions

The principal symbol of the minimal scalar equation is proportional to

$$
g^{\mu\nu}k_\mu k_\nu.
$$

Its characteristics satisfy

$$
g^{\mu\nu}k_\mu k_\nu=0.
$$

Thus the field’s wavefronts follow the null cone of the specified Lorentzian metric. A well-posed global evolution also requires suitable causal structure, initial data, and boundary conditions; a globally hyperbolic spacetime is a standard sufficient setting for the usual Cauchy problem.

In flat space the quadratic-potential dispersion relation has group velocity

$$
v_{\mathrm g}
=\frac{\partial\omega}{\partial|\mathbf k|}
=\frac{c|\mathbf k|}
{\sqrt{|\mathbf k|^2+\mu^2}}
\leq c.
$$

The characteristic wavefront speed remains $c$. In this construction the causal scale enters with the physical metric and the identification $x^0=ct$. Its deeper origin and universality have not yet been derived.

The real conservative action does not automatically produce positive entropy production or a preferred thermodynamic time direction. These may require coarse-graining, open-system dynamics, constitutive laws, additional degrees of freedom, or boundary conditions.

Likewise, $\hbar$ in a coefficient is not a quantization rule. A quantum extension would require, for example, a Hilbert-space formulation with a Hamiltonian or a defined path integral, together with a measure, state, and interpretation of observables. An entropy-weighted path-selection rule or Vuli–Ndlela-type construction would have to be specified and checked rather than inferred from the classical action alone.

## 14. A precise statement of what has been established

| Stage | Mathematical or physical status |
|---|---|
| Entropy and relative surprisal from a distribution | Definitions |
| Fisher metric from neighboring-distribution distinguishability | Derived under regularity assumptions |
| Entropy-related field as a causal substrate | ToE physical postulate |
| Four-dimensional Lorentzian metric | Geometric assumption or separately specified construction |
| Minimal local action | Model selected by stated structural assumptions |
| Scalar field equation | Derived by variation |
| Curvature-coupled field and metric equations | Derived for the stated scalar–tensor completion |
| Weighted-resistance geodesics | Derived from a separate path functional |
| Haller–Obidi rearrangement | Algebraic consequence of the stated entropy–action relation |
| Nontrivial particle localization | Requires a model-specific calculation |
| Thermodynamic irreversibility | Requires additional physical structure |
| Quantum dynamics | Requires a specified quantum extension |
| Experimental equivalence to established physics | Requires quantitative predictions and tests |

The logically ordered construction is

$$
\begin{gathered}
\text{Probability distributions}\\
\Downarrow\quad\text{definitions}\\
\text{Entropy, surprisal, and information geometry}\\
\Downarrow\quad\text{ToE physical postulates}\\
\text{Ontic entropic field and specified causal geometry}\\
\Downarrow\quad\text{locality, covariance, stability}\\
\mathcal A_{\mathrm O}\\
\Downarrow\quad\text{variation}\\
\text{Entropic field equations and geometric equations}\\
\Downarrow\quad\text{explicitly demonstrated limits}\\
\text{Effective particle and classical dynamics}.
\end{gathered}
$$

## 15. Conclusion

Obidi’s proposed starting point assigns fundamental physical significance to an entropy-related field. Once that interpretation is accompanied by a definite field variable, a geometric prescription, consistent units, and explicit dynamical assumptions, an action can be constructed and its equations derived without ambiguity. The minimal realization is a scalar-field action; a curvature-coupled completion allows the field and geometry to interact dynamically. The resistance principle and Haller–Obidi identity supply further structures whose relationship to the field theory must be demonstrated under stated assumptions. This presentation makes the entropy-first proposal intelligible while retaining the mathematical distinctions needed for a rigorous research program.

## References and verification status

1. **Obidi, J. O.** (2026). *The Theory of Entropicity (ToE) — Living Review Letters Series, Letter IB: On the Haller–Obidi Action and Lagrangian: An Examination of the Mathematical and Conceptual Connection Between John Haller’s Action-as-Entropy Equivalence and the Entropic Field Obidi Action Formulation of the Theory of Entropicity (ToE).* Cambridge Open Engage, version 1, 20 April 2026. [DOI: 10.33774/coe-2026-zfxr9](https://doi.org/10.33774/coe-2026-zfxr9). The accessible abstract confirms the stated identity and claims a localization procedure. The full localization proof was not verified for this reconstruction.
2. **Haller, J. L., Jr.** (2015). *Action as Entropy.* Proceedings of the 2nd International Electronic Conference on Entropy and Its Applications. [Conference record](https://sciforum.net/paper/view/3244); [DOI: 10.3390/ecea-2-A010](https://doi.org/10.3390/ecea-2-A010). Included for the historical entropy–action context; the exact relation discussed here is documented in reference [1].
3. **Nielsen, F.** (2020). *An Elementary Introduction to Information Geometry.* Entropy, 22(10), 1100. [DOI: 10.3390/e22101100](https://doi.org/10.3390/e22101100). Background on Fisher metrics, statistical manifolds, and Hessian structures.
4. **Tong, D.** *General Relativity*, section 4, “The Einstein Equations.” [Author’s lecture notes](https://www.damtp.cam.ac.uk/user/tong/gr/grhtml/S4.html). Background on covariant scalar actions, metric variation, and gravitational field equations.

The original supplied draft also listed *Foundations of the Theory of Entropicity (ToE): Obidi Action and Entropic Field Geometry* and *From Shannon Entropy to Obidi Action via Information Geometry*. Their exact bibliographic entries were not verified in the preceding analysis. A related work was located under the longer title *From Shannon Entropy to Spacetime: A Rigorous Derivation of the Obidi Action from Shannon Entropy via Information Geometry in the Theory of Entropicity (ToE)*, Letter IIF, but its full text was not accessible for checking. These supplied or partially located references should not be treated as independently verified support for a particular equation in this reconstruction.

---

## Appendix A. Complete preserved preceding explanation

The following preserves the preceding explanatory response. Inline mathematics uses single-dollar delimiters and display mathematics uses double-dollar delimiters. Reference markers replace the original chat citation widgets; the explanatory wording and mathematical content are retained. Numbering below reproduces the original equation numbering independently of the main paper.

The central idea can be presented coherently: **Obidi promotes an entropy-related quantity to a physical field, then constructs a variational principle governing that field and its relationship to geometry.** To make the account mathematically sound, we must distinguish the definition of entropy, the physical postulates introduced by ToE, and the equations subsequently derived from the action.

Several equations in your draft need correction. In particular, the invariant volume element is $\sqrt{-g}\,d^4x$; a squared field gradient is a kinetic term rather than geometric curvature; and the Haller–Obidi coefficient is $\hbar/2$, not $\hbar^2$.

I verified that Obidi’s Letter IB presents the Haller–Obidi relation and claims a localization correspondence. Its accessible abstract, however, does not provide enough detail to check that localization proof. The construction below is therefore **a mathematically consistent reconstruction of your supplied framework**, with additional assumptions identified explicitly, rather than a claim to reproduce every step of the cited manuscripts. [1]

We should begin by separating three quantities that your draft denotes using similar symbols:

| Symbol | Meaning | Units |
|---|---|---|
| $H$ | Dimensionless information entropy | Dimensionless |
| $S_{\mathrm{ent}}=k_BH$ | Entropy with physical units | Energy/temperature |
| $\mathcal A_{\mathrm O}$ | Obidi action | Energy × time |

For the dynamical field, write

$$
s(x)=\frac{S_{\mathrm{ent}}(x)}{k_B}.
\tag{1}
$$

Thus $s$ is dimensionless. This normalization makes it easier to check the action’s units and prevents entropy from being confused with action.

The starting point is a normalized probability distribution. For discrete alternatives,

$$
p_i\geq 0,
\qquad
\sum_i p_i=1,
$$

and Shannon entropy is

$$
H[p]=-\sum_i p_i\ln p_i.
\tag{2}
$$

The logarithm is natural, so entropy is measured in nats. The corresponding physical entropy is $k_BH$.

For continuous microstates $y$, additional care is necessary because a probability density can carry units. A coordinate-independent construction uses a positive reference density $q(y)$, defined relative to the same measure $d\mu(y)$:

$$
H_q[p]
=
-\int p(y)
\ln\!\left(\frac{p(y)}{q(y)}\right)d\mu(y).
\tag{3}
$$

The ratio inside the logarithm is dimensionless. When $q$ is normalized, this expression is the negative Kullback–Leibler divergence, rather than unrestricted ordinary Shannon entropy. Specifying the reference measure or reference density is part of the definition.

To obtain a quantity that varies across a manifold, associate a local probability distribution with each point $x$:

$$
p(y\mid x),
\qquad
\int p(y\mid x)\,d\mu(y)=1.
\tag{4}
$$

Here $x$ labels the manifold point, while $y$ labels microstates. They are different variables.

A local entropy field can then be defined by

$$
s(x)
=
-\int p(y\mid x)
\ln\!\left(\frac{p(y\mid x)}{q(y)}\right)d\mu(y).
\tag{5}
$$

This provides a statistical construction of a scalar field. It does not yet assign that field causal power.

**Obidi’s ontological postulate enters at precisely this point:** within ToE, the entropy-related field is taken to represent a physically operative substrate whose configurations participate in determining dynamics.

That physical interpretation is an additional postulate. It is not a mathematical consequence of Shannon’s entropy formula.

There is also a distinction between entropy and local surprisal. The logarithmic quantity

$$
\lambda(y,x)
=
-\ln\!\left(\frac{p(y\mid x)}{q(y)}\right)
\tag{6}
$$

is a relative surprisal, whereas

$$
s(x)=\int p(y\mid x)\lambda(y,x)\,d\mu(y)
\tag{7}
$$

is its expectation. If the intended foundational field is instead

$$
\Lambda(x)=-k_B\ln\!\left(\frac{p(x)}{p_*(x)}\right),
\tag{8}
$$

then it should be identified as a promoted logarithmic probability field. It should not be silently equated with the averaged entropy in equation (5).

Either choice can motivate a field theory, but the manuscript must specify which field the action governs.

The next question is how probability acquires geometry. Consider a smooth family of distributions $p(y\mid\theta)$, parameterized by coordinates $\theta^a$. Its Fisher information metric is

$$
G_{ab}(\theta)
=
\int p(y\mid\theta)
\frac{\partial\ln p}{\partial\theta^a}
\frac{\partial\ln p}{\partial\theta^b}
\,d\mu(y).
\tag{9}
$$

This metric measures the local distinguishability of nearby probability distributions. Under regularity conditions, the relative entropy between neighboring distributions has the expansion

$$
D_{\mathrm{KL}}
\!\left(p_\theta\Vert p_{\theta+d\theta}\right)
=
\frac12G_{ab}(\theta)\,d\theta^a d\theta^b
+
O(\|d\theta\|^3).
\tag{10}
$$

The quadratic term supplies a notion of statistical distance. This is the information-geometric foundation relevant to the proposed construction. [3]

Its positivity can be checked directly. For any vector $v^a$,

$$
v^aG_{ab}v^b
=
\int p
\left(
v^a\frac{\partial\ln p}{\partial\theta^a}
\right)^2d\mu
\geq 0.
\tag{11}
$$

Consequently, ordinary Fisher geometry is positive semidefinite, and positive definite for a regular identifiable model. It does not automatically possess the Lorentzian signature needed for relativistic spacetime.

The formula in your draft,

$$
g_{\mu\nu}^{\mathrm{ent}}
\sim
\partial_\mu\partial_\nu I,
$$

therefore needs qualification. An ordinary Hessian of an arbitrary mutual-information function is not generally a metric tensor. For an exponential family in natural parameters,

$$
p(y\mid\theta)
=
h(y)
\exp\!\left[\theta^aT_a(y)-\psi(\theta)\right],
$$

one does obtain

$$
G_{ab}=\partial_a\partial_b\psi,
\tag{12}
$$

where $\psi$ is the log-partition function. The special family and coordinate choice are essential. [3]

If the statistical parameters vary across $M$, the information metric induces a tensor

$$
h_{\mu\nu}(x)
=
G_{ab}(\theta(x))
\partial_\mu\theta^a
\partial_\nu\theta^b.
\tag{13}
$$

This is called a pullback metric. It is nondegenerate only when the map $x\mapsto\theta(x)$ has sufficient rank.

A significant consequence follows: **one scalar entropy value does not generally contain enough information to reconstruct a four-dimensional metric.** If every statistical parameter depends only on $s(x)$, then

$$
h_{\mu\nu}
=
C(s)\,\partial_\mu s\,\partial_\nu s,
\tag{14}
$$

which has rank at most one. The theory must therefore retain sufficient statistical structure, introduce additional geometric structure, or specify another metric-construction rule.

A possible Lorentzian construction illustrates the extra assumption required. Suppose $h_{\mu\nu}$ is positive definite and a preferred unit covector $n_\mu$ is supplied:

$$
h^{\mu\nu}n_\mu n_\nu=1.
$$

Then define

$$
g_{\mu\nu}
=
h_{\mu\nu}-2n_\mu n_\nu.
\tag{15}
$$

In an $h$-orthonormal frame aligned with $n$,

$$
h_{\mu\nu}
=
\operatorname{diag}(1,1,1,1),
\qquad
g_{\mu\nu}
=
\operatorname{diag}(-1,1,1,1).
$$

This is a mathematically valid signature-changing prescription. If it is used to represent the intended Obidi transformation, the theory must explain how $n_\mu$ is selected and governed. The prescription supplies Lorentzian signature; it does not by itself establish thermodynamic irreversibility.

With the field and geometric setting specified, we can construct the action.

Assume a four-dimensional Lorentzian manifold with signature

$$
(-,+,+,+).
$$

Take $x^0=ct$, so all four coordinates have dimensions of length. Let

$$
g=\det(g_{\mu\nu}).
$$

The invariant integration measure is

$$
dV_g=\sqrt{-g}\,d^4x.
\tag{16}
$$

The square root compensates for the coordinate transformation of $d^4x$. The general local action is therefore

$$
\mathcal A_{\mathrm O}
=
\frac1c\int_M
\sqrt{-g}\,
\mathcal L_{\mathrm O}\,d^4x,
\tag{17}
$$

where $\mathcal L_{\mathrm O}$ is a scalar with units of energy density. Strictly, $\sqrt{-g}\mathcal L_{\mathrm O}$ is the coordinate density.

To select a simple action, introduce the following assumptions:

- The theory is local.
- The field $s$ is a scalar.
- The action is coordinate invariant.
- The minimal field sector contains at most two derivatives in total.
- The field has a positive kinetic-energy coefficient.

Because $s$ is a scalar,

$$
\nabla_\mu s=\partial_\mu s.
$$

The simplest quadratic derivative scalar is

$$
X=g^{\mu\nu}\nabla_\mu s\nabla_\nu s.
\tag{18}
$$

A minimal action consistent with these assumptions is

$$
\boxed{
\mathcal A_{\mathrm O}^{\mathrm{min}}[s;g]
=
\frac1c
\int_M\sqrt{-g}
\left[
-\frac{\kappa}{2}
g^{\mu\nu}\nabla_\mu s\nabla_\nu s
-
U(s)
\right]d^4x,
\qquad
\kappa>0.
}
\tag{19}
$$

Here $\kappa$ controls the energetic cost of field variation, and $U(s)$ is a potential-energy density.

This construction explains the mathematical route to a minimal Obidi field action: **the entropy-first postulate identifies the physical field, while locality, covariance, derivative order, and stability constrain the form of its dynamics.**

Those assumptions do not uniquely fix $\kappa$, $U$, or every possible interaction.

The dimensions provide an immediate check:

$$
[s]=1,
\qquad
[\nabla_\mu s]=\mathrm{length}^{-1},
$$

so

$$
[\kappa]=\frac{\mathrm{energy}}{\mathrm{length}},
\qquad
[U]=\frac{\mathrm{energy}}{\mathrm{length}^3}.
\tag{20}
$$

Since $d^4x/c$ has units of volume × time, equation (19) has units of action.

Thus neither $\hbar^2$ nor $\hbar/2$, used alone as the coefficient of this dimensionless field’s spacetime gradient term, has the required dimensions. Additional scales or a different field normalization would be necessary.

The sign can also be checked. In locally flat coordinates,

$$
g^{\mu\nu}\partial_\mu s\partial_\nu s
=
-\frac{\dot s^{\,2}}{c^2}
+
|\boldsymbol\nabla s|^2.
$$

Equation (19) then gives

$$
\mathcal L_{\mathrm O}
=
\frac{\kappa}{2c^2}\dot s^{\,2}
-
\frac{\kappa}{2}|\boldsymbol\nabla s|^2
-
U(s).
\tag{21}
$$

The time-derivative contribution has the positive sign expected for a healthy scalar kinetic term.

The field equation follows by varying $s$, initially holding $g_{\mu\nu}$ fixed. Set

$$
s\longrightarrow s+\epsilon\,\delta s
$$

and require $\delta s$ to vanish on the boundary. For constant $\kappa$,

$$
\delta\mathcal A_{\mathrm O}^{\mathrm{min}}
=
\frac1c
\int_M\sqrt{-g}
\left[
-\kappa\nabla^\mu s\,\nabla_\mu\delta s
-
U'(s)\delta s
\right]d^4x.
\tag{22}
$$

Apply the product rule,

$$
\nabla_\mu
\left(\delta s\,\nabla^\mu s\right)
=
\nabla_\mu\delta s\,\nabla^\mu s
+
\delta s\,\Box_gs,
$$

where

$$
\Box_gs
=
\nabla_\mu\nabla^\mu s
=
\frac1{\sqrt{-g}}
\partial_\mu
\left(
\sqrt{-g}\,g^{\mu\nu}\partial_\nu s
\right).
\tag{23}
$$

After integration by parts, the boundary term vanishes and

$$
\delta\mathcal A_{\mathrm O}^{\mathrm{min}}
=
\frac1c
\int_M\sqrt{-g}
\left[
\kappa\Box_gs-U'(s)
\right]\delta s\,d^4x.
\tag{24}
$$

Because $\delta s$ is arbitrary in the interior,

$$
\boxed{
\kappa\Box_gs-U'(s)=0.
}
\tag{25}
$$

This is the correctly normalized field Euler–Lagrange equation for equation (19). The familiar scalar-field variational structure is standard; ToE assigns the field its entropic interpretation. [4]

As a check, choose

$$
U(s)=\frac{\kappa\mu^2}{2}s^2,
$$

with $\mu$ an inverse length. Then

$$
\Box_gs-\mu^2s=0,
$$

or, in flat spacetime,

$$
\frac1{c^2}\frac{\partial^2s}{\partial t^2}
-
\nabla^2s
+
\mu^2s=0.
\tag{26}
$$

The sign yields the usual stable massive-wave equation.

If the kinetic coefficient depends on the field, the action contains $K(s)$ instead of $\kappa$, and the result becomes

$$
\boxed{
K(s)\Box_gs
+
\frac12K'(s)(\nabla s)^2
-
U'(s)=0.
}
\tag{27}
$$

That additional term must not be omitted.

We can now clarify what “entropic curvature” means in the action. The quantity

$$
g^{\mu\nu}\nabla_\mu s\nabla_\nu s
$$

measures field variation. It is not the Ricci scalar $R[g]$, nor another curvature invariant. Calling equation (19) a curvature functional would therefore be inaccurate unless a separate, explicit definition of entropic curvature is introduced.

If the goal is to describe both entropic dynamics and dynamical geometry, a possible two-derivative extension is

$$
\boxed{
\mathcal A_{\mathrm O}[s,g]
=
\frac1c
\int_M\sqrt{-g}
\left[
\frac12F(s)R[g]
-
\frac12K(s)(\nabla s)^2
-
U(s)
\right]d^4x
+
\mathcal A_{\mathrm m}
+
\mathcal A_{\partial M}.
}
\tag{28}
$$

Here $F(s)$ controls the curvature coupling, $\mathcal A_{\mathrm m}$ describes additional matter when present, and $\mathcal A_{\partial M}$ supplies boundary terms appropriate to the boundary conditions.

This is a scalar–tensor completion of the proposed action. Its scalar equation is

$$
K\Box_gs
+
\frac12K'(\nabla s)^2
+
\frac12F'R
-
U'=0.
\tag{29}
$$

Its metric equation is

$$
F G_{\mu\nu}
=
T_{\mu\nu}^{(s)}
+
T_{\mu\nu}^{(\mathrm m)}
+
\nabla_\mu\nabla_\nu F
-
g_{\mu\nu}\Box_gF,
\tag{30}
$$

with

$$
T_{\mu\nu}^{(s)}
=
K\nabla_\mu s\nabla_\nu s
-
g_{\mu\nu}
\left[
\frac12K(\nabla s)^2+U
\right].
\tag{31}
$$

These equations assume that $s$ and $g_{\mu\nu}$ are independently varied. If the metric is constrained to be a function of information variables, that relationship must be included in the variation. One cannot impose a composite metric and simultaneously vary it as an unconstrained independent field without further justification.

For

$$
F=\frac{c^4}{8\pi G},
$$

the curvature term has Einstein–Hilbert normalization. This gives an explicit correspondence with a familiar gravitational action; deriving that value from entropic premises would be a further result.

The Principle of Least Entropic Resistance requires a separate, careful construction. Your proposed functional integrates along a path, so its variables are the path coordinates $x^\mu(\lambda)$.

To define a nonnegative resistance, first use a positive-definite metric $h_{\mu\nu}$. A Lorentzian contraction of a gradient need not be positive and therefore cannot automatically serve as a resistance norm.

Let

$$
w(x)
=
h^{\mu\nu}\partial_\mu s\,\partial_\nu s
$$

and define

$$
\mathcal R[\gamma]
=
\int_\gamma w(x)\,d\ell_h,
\qquad
d\ell_h^2=h_{\mu\nu}dx^\mu dx^\nu.
\tag{32}
$$

For a parameterized path,

$$
\mathcal R[x]
=
\int
w(x)
\sqrt{h_{\mu\nu}\dot x^\mu\dot x^\nu}
\,d\lambda.
\tag{33}
$$

The corresponding path Lagrangian is

$$
L_\gamma(x,\dot x)
=
w(x)\sqrt{h_{\mu\nu}\dot x^\mu\dot x^\nu}.
$$

Therefore the correct Euler–Lagrange equation is

$$
\boxed{
\frac{d}{d\lambda}
\left(
\frac{\partial L_\gamma}{\partial\dot x^\mu}
\right)
-
\frac{\partial L_\gamma}{\partial x^\mu}
=0.
}
\tag{34}
$$

The derivative is taken with respect to path velocity $\dot x^\mu$, not the field gradient $\partial_\mu s$.

Parameterizing by $h$-arc length and defining the unit tangent

$$
T^\mu=\frac{dx^\mu}{d\ell_h},
\qquad
h_{\mu\nu}T^\mu T^\nu=1,
$$

gives

$$
\boxed{
w\,T^\nu\nabla^{(h)}_\nu T^\mu
=
\left(h^{\mu\nu}-T^\mu T^\nu\right)\partial_\nu w.
}
\tag{35}
$$

This equation says that the path bends in response to the component of the resistance gradient perpendicular to its tangent.

Where $w>0$, equation (32) is the length functional of the conformally rescaled metric

$$
\widetilde h_{\mu\nu}=w^2h_{\mu\nu}.
\tag{36}
$$

Thus stationary resistance paths are geodesics of $\widetilde h_{\mu\nu}$, understood as unparameterized curves.

If $w=0$, that metric degenerates. A strictly positive alternative, introduced as an additional modeling choice, is

$$
w=w_0+\ell_*^2h^{\mu\nu}\partial_\mu s\partial_\nu s,
\qquad
w_0>0.
\tag{37}
$$

Two logical qualifications are necessary. First, $\delta\mathcal R=0$ establishes stationarity; proving a minimum requires further analysis. Second, this path variational principle is not automatically equivalent to the spacetime field action. Connecting them requires a specified particle, ray, or collective-coordinate limit.

The Haller–Obidi relation can now be treated without conflating an entropy identity with a field equation.

The relation presented in Obidi’s Letter IB is

$$
H(t)-H(t_0)
=
\frac2\hbar
\int_{t_0}^{t}
\left(mc^2-L\right)dt'.
\tag{38}
$$

Differentiating and rearranging gives

$$
\boxed{
L_{\mathrm{HO}}
=
mc^2-\frac{\hbar}{2}\frac{dH}{dt}.
}
\tag{39}
$$

This matches the coefficient in the accessible abstract. [1]

The units are consistent because $H$ is dimensionless:

$$
\left[\hbar\frac{dH}{dt}\right]
=
(\mathrm{energy}\times\mathrm{time})
\times\mathrm{time}^{-1}
=
\mathrm{energy}.
$$

If physical entropy is used instead,

$$
L_{\mathrm{HO}}
=
mc^2
-
\frac{\hbar}{2k_B}
\frac{dS_{\mathrm{ent}}}{dt}.
\tag{40}
$$

However, suppose $H$ is identified with a prescribed local scalar evaluated along a trajectory:

$$
H(t)=s(x(t)).
$$

Then the chain rule gives

$$
\frac{dH}{dt}
=
\partial_t s+\dot x^i\partial_i s,
$$

so

$$
\mathcal A_{\mathrm{HO}}
=
mc^2(t_f-t_i)
-
\frac{\hbar}{2}
\left[s(x_f)-s(x_i)\right].
\tag{41}
$$

For fixed spacetime endpoints and constant mass, this expression is independent of the interior path. **The entropy derivative contributes only a boundary term and supplies no bulk force.**

This does not invalidate every possible entropy–action correspondence. It establishes that a nontrivial correspondence must specify whether $H$ is an accumulated, path-dependent entropy functional rather than merely the value of a local scalar. For example, a rate

$$
\frac{dH}{dt}=r(x,\dot x,t)
$$

can influence motion if its integral is genuinely path dependent and cannot be reduced to fixed endpoint values.

The covariant expression needs the same care. With proper time $\tau$,

$$
u^\mu=\frac{dx^\mu}{d\tau},
\qquad
u^\mu\nabla_\mu s=\frac{ds}{d\tau},
$$

and hence

$$
\int u^\mu\nabla_\mu s\,d\tau=s_f-s_i.
\tag{42}
$$

It remains a boundary contribution. Moreover, replacing $dt$ with $d\tau$ is not merely a notation change; a relativistic worldline action must be formulated consistently.

A standard effective particle action is

$$
\mathcal A_{\mathrm{pp}}=-mc^2\int d\tau.
\tag{43}
$$

To derive this from an entropic field theory, one would need a localized field configuration, substitute its moving profile into the field action, integrate over its spatial structure, and demonstrate that the resulting effective action has equation (43)’s form.

Once that result is obtained, its nonrelativistic expansion is

$$
L_{\mathrm{pp}}
=
-mc^2\sqrt{1-\frac{v^2}{c^2}}
=
-mc^2+\frac12mv^2
+
O\!\left(\frac{mv^4}{c^2}\right).
\tag{44}
$$

Dropping the constant rest-energy term recovers the usual free-particle kinetic Lagrangian. This makes the required localization argument concrete.

Finally, the conservation and causal claims must follow from specified structures.

For the minimal action, the stress tensor is equation (31) with $K=\kappa$, and direct differentiation gives

$$
\nabla^\mu T_{\mu\nu}^{(s)}
=
\left(\kappa\Box_gs-U'(s)\right)\nabla_\nu s.
\tag{45}
$$

It is conserved when the field equation holds and the scalar sector has no exchange with additional fields.

A conserved scalar current requires a symmetry. For constant $U$, the action is invariant under constant shifts of $s$, and one may take

$$
J^\mu=\kappa\nabla^\mu s,
\qquad
\nabla_\mu J^\mu=0.
\tag{46}
$$

For nonconstant $U$,

$$
\nabla_\mu J^\mu=U'(s).
\tag{47}
$$

A thermodynamic entropy current is a different object. If it is modeled as

$$
J_S^\mu=\rho_Su^\mu,
$$

its balance law generally takes the form

$$
\nabla_\mu J_S^\mu=\sigma,
\qquad
\sigma\geq0,
\tag{48}
$$

where $\sigma$ is entropy production. Conservation is the special case $\sigma=0$. The existence of a scalar action alone does not establish this thermodynamic interpretation.

Likewise, equation (25) has a principal differential part determined by $g^{\mu\nu}$, so its characteristics satisfy

$$
g^{\mu\nu}k_\mu k_\nu=0.
\tag{49}
$$

Its wavefronts therefore follow the metric’s null cone. Calling $c$ the maximum entropic propagation speed is consistent with this model, but the value and universality of $c$ have been supplied through the Lorentzian structure. Deriving them from deeper entropic assumptions requires another argument.

Irreversibility and quantum behavior also require additional structure. A real scalar action can describe time-reversal-invariant classical dynamics, and inserting $\hbar$ into a coefficient does not itself quantize the theory.

The logically defensible hierarchy is therefore

$$
\boxed{
\begin{gathered}
\text{Probability distributions}
\\
\Downarrow\quad\text{definitions}
\\
\text{Entropy, surprisal, and information geometry}
\\
\Downarrow\quad\text{ToE physical postulates}
\\
\text{Ontic entropic field and specified causal geometry}
\\
\Downarrow\quad\text{locality, covariance, stability}
\\
\mathcal A_{\mathrm O}
\\
\Downarrow\quad\text{variation}
\\
\text{Entropic field equations and geometric equations}
\\
\Downarrow\quad\text{explicitly demonstrated limits}
\\
\text{Effective particle and classical dynamics}.
\end{gathered}
}
\tag{50}
$$

The foundational claim can accordingly be written as follows:

Within the Theory of Entropicity, Obidi proposes that an entropy-related field constitutes a primary physical substrate. Probability theory supplies candidate field variables, and information geometry supplies structures measuring distinguishability. Once the field’s ontological status, the geometric prescription, and the dynamical assumptions are specified, a covariant action can be constructed and varied to obtain field equations. Its minimal realization is an entropic scalar-field action; a curvature-coupled extension allows the field and geometry to interact dynamically. Correspondence with particle mechanics, thermodynamic irreversibility, and quantum theory must then be established through explicit reductions or additional principles. This formulation identifies exactly where Obidi’s physical proposal enters and exactly which mathematical consequences follow from it.

## Appendix B. Qualifications that apply to the preserved explanation

The main paper supplies the following additional precision without removing or rewriting the preserved explanation:

1. Equation (29) assumes that $\mathcal A_{\mathrm m}$ has no explicit dependence on $s$. Otherwise its scalar variation supplies another source term.
2. The conserved shift current in equation (46) belongs to the minimal model with constant $\kappa$ and constant $U$. It is not automatically a thermodynamic entropy current or a symmetry of a nonminimally coupled model.
3. Equation (45) concerns the minimally coupled scalar sector. With nonconstant $F$, the scalar stress tensor alone generally exchanges energy-momentum with the curvature-coupling sector.
4. The positivity requirement on $\kappa$ fixes the kinetic sign. A lower bound on $U$, appropriate background conditions, and any additional coupled-field stability conditions must also be checked.
5. Equation (36) identifies unparameterized weighted-length geodesics where $w>0$. A reference weight can restore conventional dimensionless metric components when $w$ carries units.
6. The positive weight in equation (37) changes the model. It cures degeneracy but does not establish equivalence with the original unregularized functional.
7. A proper-time integral of $mc^2$ is path dependent. The no-bulk-force conclusion in equation (41) concerns the stated coordinate-time action with fixed spacetime endpoints and constant mass; the entropy total derivative is a boundary term in either parametrization.
8. Fisher differentiation identities presume smoothness, suitable support, and valid interchange of differentiation and integration. Boundary or support-dependent contributions must be considered when these conditions fail.
9. A scalar defined as an average over probabilities is a composite quantity. Treating it as an independently variable effective field requires an explicit effective-theory assumption or a derivation from the probability variables.
10. Four-dimensionality, a Lorentzian causal prescription, the dynamics of the selected time direction, and the identification of the physical speed $c$ remain specified inputs until independently derived.
