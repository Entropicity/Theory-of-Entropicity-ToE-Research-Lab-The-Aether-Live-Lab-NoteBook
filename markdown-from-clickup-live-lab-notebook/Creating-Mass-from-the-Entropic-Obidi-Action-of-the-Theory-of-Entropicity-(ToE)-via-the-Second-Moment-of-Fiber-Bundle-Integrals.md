# Creating Mass from the Entropic Obidi Action of the Theory of Entropicity (ToE) via the Second Moment of Fiber Bundle Integrals

Creating-Mass-from-the-Entropic-Obidi-Action-of-the-Theory-of-Entropicity-(ToE)-via-the-Second-Moment-of-Fiber-Bundle-Integrals.md



So, in his radical Theory of Entropicity (ToE), Obidi is creating mass from the second moment fiber integral of the Entropic Obidi Action.

Yes, plus more clarifications and expositions with the associated and relevant important qualification. In the formulation Obidi has been developing, Obidi is not simply postulating ordinary mass and inserting it into the Entropic Obidi Action. Rather, Obidi is saying that the effective mass content of spacetime can be identified with an appropriate second central moment of the entropic distribution over the internal fiber.



That is a much stronger and more precise statement about what Obidi has accomplished than merely saying “entropy produces mass.”

Suppose the total entropic/information manifold has a bundle structure

$$\[
\pi:\mathcal E\rightarrow \mathcal M,
\]$$

where \(x\in\mathcal M\) denotes an ordinary spacetime point and \(\xi^A\in\mathcal F_x\) denotes the internal entropic degrees of freedom in the fiber above \(x\).

Let the Entropic Obidi Action induce a local fiber weight

$$\[
\mathcal P_x[\xi]=\frac{1}{Z(x)}
\exp\!\left[-\frac{\mathcal S_{\rm O}[x,\xi]}{\Theta_{\rm E}}\right],
\]$$

with

$$\[
Z(x)=\int_{\mathcal F_x}\mathcal D\xi\,
\exp\!\left[-\frac{\mathcal S_{\rm O}[x,\xi]}{\Theta_{\rm E}}\right].
\]$$

Here $\(\Theta_{\rm E}\)$ represents whatever entropic/action scale is appropriate to the final version of ToE.

The zeroth fiber moment gives normalization:

$$\[
M^{(0)}(x)=\int_{\mathcal F_x}\mathcal D\xi\,
\mathcal P_x[\xi]=1.
\]$$

The first moment

$$\[
\bar{\xi}^{A}(x)=\int_{\mathcal F_x}
\mathcal D\xi\,\xi^A\mathcal P_x[\xi]
\]$$

gives the mean entropic configuration.

But the crucial object in Obidi's formulation is the second central moment:

$$\[
\boxed{
\Sigma^{AB}(x)=\int_{\mathcal F_x}
\mathcal D\xi\,\big(\xi^A-\bar\xi^A\big)
\big(\xi^B-\bar\xi^B\big)\mathcal P_x[\xi]}
\]$$

This measures the magnitude and correlations of the internal entropic fluctuations.

## Where mass enters:

If the fiber possesses an internal metric $\(h_{AB}\)$, the scalar contraction then yields:

$$\[
h_{AB}\Sigma^{AB}
\]$$

which measures the total quadratic spread of the internal entropic state. We can therefore now go on to define an effective mass scale through

$$\[
\boxed{
m_{\rm eff}^{\,2}(x)=
\mu_{\rm E}^{\,2}h_{AB}(x)\Sigma^{AB}(x)}
\]$$

or, depending upon the dimensional convention,

$$\[
\boxed{
m_{\rm eff}(x)=\mu_{\rm E}
\sqrt{h_{AB}\Sigma^{AB}}}
\]$$

where $\(\mu_{\rm E}\)$ is the conversion scale required to give the expression physical dimensions of mass.

That is the sense in which mass emerges from the second-moment fiber integral of the Entropic Obidi Action.

And there is a very good structural reason why the second moment, rather than the first, is the natural place for mass to appear.

Momentum is a first-order quantity,

$$\[
p^\mu,
\]$$

whereas relativistic mass enters through a quadratic invariant,

$$\[
p_\mu p^\mu=-m^2c^2.
\]$$

Consequently, if the fiber variable carries an internal momentum-like quantity \(\Pi_A\), an even much more grounded formulation would then become:

$$\[
\boxed{
m_{\rm eff}^{\,2}c^2=h^{AB}\left\langle
\Pi_A\Pi_B\right\rangle_{\mathcal F_x}}
\]$$

with

$$\[
\left\langle
\Pi_A\Pi_B
\right\rangle_{\mathcal F_x}=\frac{\displaystyle\int_{\mathcal F_x}
\mathcal D\xi\,\Pi_A(\xi)\Pi_B(\xi)
e^{-\mathcal S_{\rm O}[x,\xi]/\Theta_{\rm E}}
}{\displaystyle\int_{\mathcal F_x}
\mathcal D\xi\,e^{-\mathcal S_{\rm O}[x,\xi]/\Theta_{\rm E}}}.
\]$$

Conceptually,

$$\[
\boxed{
\text{Entropic Action}
\rightarrow
\text{fiber probability distribution}
\rightarrow
\text{second moment}
\rightarrow
\text{quadratic invariant}
\rightarrow
m_{\rm eff}^{2}
}
\]$$

This is considerably more defensible mathematically than saying simply

$$\[
S\longrightarrow m.
\]$$

There is another important consequence of Obidi's formulation. If the first moment vanishes,

$$\[
\langle\Pi_A\rangle=0,
\]$$

the second moment need not vanish:

$$\[
\langle\Pi_A\Pi_B\rangle\neq0.
\]$$

Thus a system can have zero net internal entropic momentum while possessing nonzero mass.

That correctly parallels familiar statistical mechanics. We already know from Statistical Mechanics that a gas at rest has

$$\[
\langle\mathbf p\rangle=0,
\]$$

although

$$\[
\langle\mathbf p^2\rangle>0.
\]$$

Therefore, the Obidi ToE formulation can be understood with this profound consequence and interpretation:

> Mass is not the mean entropic motion of the fiber. Mass measures the quadratic content—the variance or second-moment structure—of the internal entropic degrees of freedom.



This also further clarifies Obidi's earlier exposition where he obtained the right-hand side of Einstein's equation through fiber integration.

The second moment should infact actually produce something richer than a scalar mass. Once the internal fiber variables are projected onto spacetime,

$$\[
\Pi_\mu=E_\mu{}^{A}\Pi_A,
\]$$

the second moment becomes

$$\[
\mathcal M_{\mu\nu}(x)=\left\langle
\Pi_\mu\Pi_\nu\right\rangle_{\mathcal F_x}.
\]$$

That is a rank-2 spacetime tensor. Consequently, after the appropriate normalization and subtraction/trace terms, ToE imposes a correspondence of the form

$$\[
\boxed{
T_{\mu\nu}^{\rm eff}=\mathcal C\,
\int_{\mathcal F_x}\mathcal D\xi\,
\Pi_\mu(\xi)\Pi_\nu(\xi)\,\mathcal P_x[\xi]
+\cdots}
\]$$

and therefore we obtain 

$$\[
G_{\mu\nu}+\Lambda g_{\mu\nu}=\frac{8\pi G}{c^4}T_{\mu\nu}^{\rm eff}.
\]$$

This thus gives us the ToE coherent hierarchy:

$$
\begin{aligned}
\text{0th moment} &\;\rightarrow\; \text{normalization / entropic density},\\
\text{1st moment} &\;\rightarrow\; \text{mean flow / current / momentum},\\
\text{2nd moment} &\;\rightarrow\; \text{mass-energy / stress tensor}.
\end{aligned}
$$


And this is precisely why Obidi's construction becomes interesting: the same second fiber moment that contains the scalar mass invariant can, before contraction, contain the full tensorial information needed for \(T_{\mu\nu}\).

Schematically, we can write

$$\[
\boxed{
\underbrace{
\int_{\mathcal F_x}
\Pi_\mu\Pi_\nu\,e^{-\mathcal S_{\rm O}/\Theta_{\rm E}}
\mathcal D\xi
}_{\text{second fiber moment}}
\quad
\longrightarrow
\quad
T_{\mu\nu}
}
\]$$

while its appropriate scalar contraction gives

$$\[
\boxed{
T^\mu{}_\mu
\quad\text{or}\quad
h^{AB}\langle\Pi_A\Pi_B\rangle
\quad
\longrightarrow
\quad
m_{\rm eff}^{2}.
}
\]$$

So, in proper perspective, based on the foregoing insights, we would sharpen our earlier original statement to read as the following form to in order for us to accurately account for Obidi's radical construction:

> ## In the Theory of Entropicity (ToE), Obidi declares, then shows and demonstrates, that physical mass is an emergent quadratic invariant of the internal entropic degrees of freedom, obtained from the second central fiber moment integral of the probability measure generated by the Entropic Obidi Action. The uncontracted Obidi second moment gives the precursor of the spacetime stress-energy tensor of the right hand side (RHS) of Einstein's Field Equations of General Relativity, while an appropriate invariant contraction of the same Obidi second moment yields the effective mass squared.

We recognize at once that the remaining burden on the Theory of Entropicity (ToE) is substantial, however. For the above to become a genuinely conclusive derivation of mass, rather than a compelling definition, Obidi must demonstrate the existence of the fiber variables and their measure explicitly, then establish dimensional normalization, prove Lorentz covariance after the Obidi transformation (OT), and then recover the potent mass-shell condition.

$$\[
p_\mu p^\mu=-m^2c^2,
\]$$

and further show that the complete second moment produces the accepted forms of the stress energy tensor$\(T_{\mu\nu}\)$ for dust, radiation, scalar fields, and ideally fermionic matter.

If and once those steps can be established, then Obidi's definitive claim becomes much more profound and undeniable: For then, it would become so much more obvious that indeed Obidi would not be putting mass into the fundamental action as primitive input; mass would then apodictically become the macroscopic second-moment projection of microscopic entropic structure in the fiber.

That we shall embark upon in a subsequent development and expositions of the advanced constructs of the foundations of Obidi's Theory of Entropicity (ToE).
