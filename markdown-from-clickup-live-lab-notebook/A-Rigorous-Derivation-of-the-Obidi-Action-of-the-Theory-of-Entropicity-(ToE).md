
# A Rigorous Derivation of the Obidi Action of the Theory of Entropicity (ToE)

 A-Rigorous-Derivation-of-the-Obidi-Action-of-the-Theory-of-Entropicity-(ToE).md

The central idea can be presented coherently: **Obidi promotes an entropy-related quantity to a physical field, then constructs a variational principle governing that field and its relationship to geometry.** To make the account mathematically sound, we must distinguish the definition of entropy, the physical postulates introduced by ToE, and the equations subsequently derived from the action.

Several equations in your draft need correction. In particular, the invariant volume element is \(\sqrt{-g}\,d^4x\); a squared field gradient is a kinetic term rather than geometric curvature; and the Haller–Obidi coefficient is \(\hbar/2\), not \(\hbar^2\).

I verified that Obidi’s Letter IB presents the Haller–Obidi relation and claims a localization correspondence. Its accessible abstract, however, does not provide enough detail to check that localization proof. The construction below is therefore **a mathematically consistent reconstruction of your supplied framework**, with additional assumptions identified explicitly, rather than a claim to reproduce every step of the cited manuscripts. ([Cambridge Open Engage][1])

We should begin by separating three quantities that your draft denotes using similar symbols:

| Symbol                     | Meaning                           | Units              |
| -------------------------- | --------------------------------- | ------------------ |
| \(H\)                      | Dimensionless information entropy | Dimensionless      |
| \(S_{\mathrm{ent}}=k_BH\)  | Entropy with physical units       | Energy/temperature |
| \(\mathcal A_{\mathrm O}\) | Obidi action                      | Energy × time      |

For the dynamical field, write

$$
s(x)=\frac{S_{\mathrm{ent}}(x)}{k_B}.
\tag{1}
$$

Thus \(s\) is dimensionless. This normalization makes it easier to check the action’s units and prevents entropy from being confused with action.

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

The logarithm is natural, so entropy is measured in nats. The corresponding physical entropy is \(k_BH\).

For continuous microstates \(y\), additional care is necessary because a probability density can carry units. A coordinate-independent construction uses a positive reference density \(q(y)\), defined relative to the same measure \(d\mu(y)\):

$$
H_q[p]
=
-\int p(y)
\ln\!\left(\frac{p(y)}{q(y)}\right)d\mu(y).
\tag{3}
$$

The ratio inside the logarithm is dimensionless. When \(q\) is normalized, this expression is the negative Kullback–Leibler divergence, rather than unrestricted ordinary Shannon entropy. Specifying the reference measure or reference density is part of the definition.

To obtain a quantity that varies across a manifold, associate a local probability distribution with each point \(x\):

$$
p(y\mid x),
\qquad
\int p(y\mid x)\,d\mu(y)=1.
\tag{4}
$$

Here \(x\) labels the manifold point, while \(y\) labels microstates. They are different variables.

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

The next question is how probability acquires geometry. Consider a smooth family of distributions \(p(y\mid\theta)\), parameterized by coordinates \(\theta^a\). Its Fisher information metric is

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

The quadratic term supplies a notion of statistical distance. This is the information-geometric foundation relevant to the proposed construction. ([PMC][2])

Its positivity can be checked directly. For any vector \(v^a\),

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

where \(\psi\) is the log-partition function. The special family and coordinate choice are essential. ([mdpi.com][3])

If the statistical parameters vary across \(M\), the information metric induces a tensor

$$
h_{\mu\nu}(x)
=
G_{ab}(\theta(x))
\partial_\mu\theta^a
\partial_\nu\theta^b.
\tag{13}
$$

This is called a pullback metric. It is nondegenerate only when the map \(x\mapsto\theta(x)\) has sufficient rank.

A significant consequence follows: **one scalar entropy value does not generally contain enough information to reconstruct a four-dimensional metric.** If every statistical parameter depends only on \(s(x)\), then

$$
h_{\mu\nu}
=
C(s)\,\partial_\mu s\,\partial_\nu s,
\tag{14}
$$

which has rank at most one. The theory must therefore retain sufficient statistical structure, introduce additional geometric structure, or specify another metric-construction rule.

A possible Lorentzian construction illustrates the extra assumption required. Suppose \(h_{\mu\nu}\) is positive definite and a preferred unit covector \(n_\mu\) is supplied:

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

In an \(h\)-orthonormal frame aligned with \(n\),

$$
h_{\mu\nu}
=
\operatorname{diag}(1,1,1,1),
\qquad
g_{\mu\nu}
=
\operatorname{diag}(-1,1,1,1).
$$

This is a mathematically valid signature-changing prescription. If it is used to represent the intended Obidi transformation, the theory must explain how \(n_\mu\) is selected and governed. The prescription supplies Lorentzian signature; it does not by itself establish thermodynamic irreversibility.

With the field and geometric setting specified, we can construct the action.

Assume a four-dimensional Lorentzian manifold with signature

$$
(-,+,+,+).
$$

Take \(x^0=ct\), so all four coordinates have dimensions of length. Let

$$
g=\det(g_{\mu\nu}).
$$

The invariant integration measure is

$$
dV_g=\sqrt{-g}\,d^4x.
\tag{16}
$$

The square root compensates for the coordinate transformation of \(d^4x\). The general local action is therefore

$$
\mathcal A_{\mathrm O}
=
\frac1c\int_M
\sqrt{-g}\,
\mathcal L_{\mathrm O}\,d^4x,
\tag{17}
$$

where \(\mathcal L_{\mathrm O}\) is a scalar with units of energy density. Strictly, \(\sqrt{-g}\mathcal L_{\mathrm O}\) is the coordinate density.

To select a simple action, introduce the following assumptions:

* The theory is local.
* The field \(s\) is a scalar.
* The action is coordinate invariant.
* The minimal field sector contains at most two derivatives in total.
* The field has a positive kinetic-energy coefficient.

Because \(s\) is a scalar,

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

Here \(\kappa\) controls the energetic cost of field variation, and \(U(s)\) is a potential-energy density.

This construction explains the mathematical route to a minimal Obidi field action: **the entropy-first postulate identifies the physical field, while locality, covariance, derivative order, and stability constrain the form of its dynamics.**

Those assumptions do not uniquely fix \(\kappa\), \(U\), or every possible interaction.

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

Since \(d^4x/c\) has units of volume × time, equation (19) has units of action.

Thus neither \(\hbar^2\) nor \(\hbar/2\), used alone as the coefficient of this dimensionless field’s spacetime gradient term, has the required dimensions. Additional scales or a different field normalization would be necessary.

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

The field equation follows by varying \(s\), initially holding \(g_{\mu\nu}\) fixed. Set

$$
s\longrightarrow s+\epsilon\,\delta s
$$

and require \(\delta s\) to vanish on the boundary. For constant \(\kappa\),

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

Because \(\delta s\) is arbitrary in the interior,

$$
\boxed{
\kappa\Box_gs-U'(s)=0.
}
\tag{25}
$$

This is the correctly normalized field Euler–Lagrange equation for equation (19). The familiar scalar-field variational structure is standard; ToE assigns the field its entropic interpretation. ([damtp.cam.ac.uk][4])

As a check, choose

$$
U(s)=\frac{\kappa\mu^2}{2}s^2,
$$

with \(\mu\) an inverse length. Then

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

If the kinetic coefficient depends on the field, the action contains \(K(s)\) instead of \(\kappa\), and the result becomes

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

measures field variation. It is not the Ricci scalar \(R[g]\), nor another curvature invariant. Calling equation (19) a curvature functional would therefore be inaccurate unless a separate, explicit definition of entropic curvature is introduced.

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

Here \(F(s)\) controls the curvature coupling, \(\mathcal A_{\mathrm m}\) describes additional matter when present, and \(\mathcal A_{\partial M}\) supplies boundary terms appropriate to the boundary conditions.

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

These equations assume that \(s\) and \(g_{\mu\nu}\) are independently varied. If the metric is constrained to be a function of information variables, that relationship must be included in the variation. One cannot impose a composite metric and simultaneously vary it as an unconstrained independent field without further justification.

For

$$
F=\frac{c^4}{8\pi G},
$$

the curvature term has Einstein–Hilbert normalization. This gives an explicit correspondence with a familiar gravitational action; deriving that value from entropic premises would be a further result.

The Principle of Least Entropic Resistance requires a separate, careful construction. Your proposed functional integrates along a path, so its variables are the path coordinates \(x^\mu(\lambda)\).

To define a nonnegative resistance, first use a positive-definite metric \(h_{\mu\nu}\). A Lorentzian contraction of a gradient need not be positive and therefore cannot automatically serve as a resistance norm.

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

The derivative is taken with respect to path velocity \(\dot x^\mu\), not the field gradient \(\partial_\mu s\).

Parameterizing by \(h\)-arc length and defining the unit tangent

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

Where \(w>0\), equation (32) is the length functional of the conformally rescaled metric

$$
\widetilde h_{\mu\nu}=w^2h_{\mu\nu}.
\tag{36}
$$

Thus stationary resistance paths are geodesics of \(\widetilde h_{\mu\nu}\), understood as unparameterized curves.

If \(w=0\), that metric degenerates. A strictly positive alternative, introduced as an additional modeling choice, is

$$
w=w_0+\ell_*^2h^{\mu\nu}\partial_\mu s\partial_\nu s,
\qquad
w_0>0.
\tag{37}
$$

Two logical qualifications are necessary. First, \(\delta\mathcal R=0\) establishes stationarity; proving a minimum requires further analysis. Second, this path variational principle is not automatically equivalent to the spacetime field action. Connecting them requires a specified particle, ray, or collective-coordinate limit.

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

This matches the coefficient in the accessible abstract. ([Cambridge Open Engage][1])

The units are consistent because \(H\) is dimensionless:

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

However, suppose \(H\) is identified with a prescribed local scalar evaluated along a trajectory:

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

This does not invalidate every possible entropy–action correspondence. It establishes that a nontrivial correspondence must specify whether \(H\) is an accumulated, path-dependent entropy functional rather than merely the value of a local scalar. For example, a rate

$$
\frac{dH}{dt}=r(x,\dot x,t)
$$

can influence motion if its integral is genuinely path dependent and cannot be reduced to fixed endpoint values.

The covariant expression needs the same care. With proper time \(\tau\),

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

It remains a boundary contribution. Moreover, replacing \(dt\) with \(d\tau\) is not merely a notation change; a relativistic worldline action must be formulated consistently.

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

For the minimal action, the stress tensor is equation (31) with \(K=\kappa\), and direct differentiation gives

$$
\nabla^\mu T_{\mu\nu}^{(s)}
=
\left(\kappa\Box_gs-U'(s)\right)\nabla_\nu s.
\tag{45}
$$

It is conserved when the field equation holds and the scalar sector has no exchange with additional fields.

A conserved scalar current requires a symmetry. For constant \(U\), the action is invariant under constant shifts of \(s\), and one may take

$$
J^\mu=\kappa\nabla^\mu s,
\qquad
\nabla_\mu J^\mu=0.
\tag{46}
$$

For nonconstant \(U\),

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

where \(\sigma\) is entropy production. Conservation is the special case \(\sigma=0\). The existence of a scalar action alone does not establish this thermodynamic interpretation.

Likewise, equation (25) has a principal differential part determined by \(g^{\mu\nu}\), so its characteristics satisfy

$$
g^{\mu\nu}k_\mu k_\nu=0.
\tag{49}
$$

Its wavefronts therefore follow the metric’s null cone. Calling \(c\) the maximum entropic propagation speed is consistent with this model, but the value and universality of \(c\) have been supplied through the Lorentzian structure. Deriving them from deeper entropic assumptions requires another argument.

Irreversibility and quantum behavior also require additional structure. A real scalar action can describe time-reversal-invariant classical dynamics, and inserting \(\hbar\) into a coefficient does not itself quantize the theory.

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

[1]: https://www.cambridge.org/engage/coe/article-details/69e5ddf3810b9dcc824e10b0?utm_source=chatgpt.com "THE THEORY OF ENTROPICITY (ToE) - LIVING REVIEW LETTERS SERIES, Letter IB: On the Haller-Obidi Action and Lagrangian: An Examination of the Mathematical and Conceptual Connection Between John Haller's Action-as-Entropy Equivalence and the Entropic Field Obidi Action Formulation of the Theory of Entropicity (ToE) | Physics and Astronomy"
[2]: https://pmc.ncbi.nlm.nih.gov/articles/PMC7650632/?utm_source=chatgpt.com "An Elementary Introduction to Information Geometry"
[3]: https://www.mdpi.com/1099-4300/22/10/1100?utm_source=chatgpt.com "An Elementary Introduction to Information Geometry"
[4]: https://www.damtp.cam.ac.uk/user/tong/gr/grhtml/S4.html?utm_source=chatgpt.com "4 The Einstein Equations‣ General Relativity by David Tong"
