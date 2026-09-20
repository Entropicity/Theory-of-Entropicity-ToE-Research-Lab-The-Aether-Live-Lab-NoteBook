# Technical questions and possible refinements to the Theory of Entropicity (ToE): Daniel Moses Alemoh's Contributions to the Development of ToE

Technical-questions-and-possible-refinements-to-the-Theory-of-Entropicity-(ToE)-Daniel-Moses-Alemoh's-Contributions-to-the-Development-of-ToE.md


---------- Forwarded message ---------

From: Daniel Alemoh <danielalemoh2@gmail.com>

Date: Thu, Sep 17, 2026 at 4:18 PM

## Subject: Technical questions and possible refinements to the Theory of Entropicity

To: JOHN OBIDI <jonimisiobidi@gmail.com>


**Dear Dr. Obidi,**

I hope you are doing very well.

I have been following your recent development of the Theory of Entropicity (ToE), particularly the Living Review Letters and, most recently, Letter III, “From Information Geometry to Information Gravity: Information Geometry as the Origin of Einstein’s Gravity.”

I want to say at the outset that I am approaching this from the position of an interested but non-specialist reader. I do not have the mathematical training required to independently verify the differential geometry, variational calculus, or field-theoretic derivations in your work. Because I wanted to understand the mathematical structure more seriously, I used an AI system as a kind of preliminary mathematical screening tool: I fed it portions of the framework and asked it to identify possible logical stress points, limiting cases, counterexamples, hidden assumptions, and places where the distinction between a mathematical construction and a first-principles physical derivation might need to be made especially explicit.

I am therefore not presenting the observations below as objections that I believe I have proved. Rather, I am sending them to you because they seemed sufficiently important that, if valid, addressing them explicitly could make ToE substantially stronger and easier for the wider mathematical-physics community to evaluate.

In particular, I think the following points may be worth incorporating into future revisions of Letter III and the other ToE publications.

## THE OBlDI TRANSFORMATION AND THE ORIGIN OF THE LORENTZIAN SIGNATURE

The central transformation is presented in the form

G̃_ab = G_ab − 2 (∇_a S ∇_b S)/(G^cd ∇_c S ∇_d S).

Equivalently, defining

u_a = ∇_a S / √(G^cd ∇_c S ∇_d S),

we have

G̃_ab = G_ab − 2 u_a u_b,

with

G^ab u_a u_b = 1.

The mathematical signature change appears clear: if G_ab is positive definite and u_a is normalized, the eigenvalue in the u-direction changes from +1 to −1.

However, this raises what seems to me to be a foundational question.

More generally, one could write

G̃_ab = G_ab − λ u_a u_b.

The eigenvalue in the u-direction then becomes

1 − λ.

Thus:

λ < 1 → positive definite,
λ = 1 → degenerate,
λ > 1 → Lorentzian.

The value λ = 2 gives the familiar normalization −1, but the signature change itself only requires λ > 1.

Could ToE therefore provide a dynamical or variational derivation of λ = 2, rather than taking it as the minimal geometric operation?

For example, is there a deeper principle in the Obidi Action, entropy dynamics, causality, stability, or information geometry that uniquely selects

λ = 2

rather than an arbitrary λ > 1?

If such a derivation exists, I think making it completely explicit would greatly strengthen the theory.

Otherwise, a reader may reasonably distinguish between:

“the entropy gradient provides the distinguished temporal direction”

and

“the entropy dynamics necessarily produces precisely the Lorentzian metric.”

The first seems to follow naturally from the construction; the second requires the uniqueness of the transformation to be demonstrated.

THE ∇S = 0 PROBLEM

A second issue concerns the normalization

u_a = ∇_a S / |∇S|.

This requires

∇_a S ≠ 0.

At an entropy critical point,

∇S = 0,

the normalized vector becomes undefined (formally 0/0), and therefore

G̃_ab = G_ab − 2 u_a u_b

is also undefined.

Since a fundamental scalar field can in principle have extrema or stationary regions, could ToE explicitly state the mathematical and physical treatment of such points?

For example:

• Are critical points excluded from the physical manifold?

• Are they treated as boundaries?

• Is there another definition of the emergent metric at such points?

• Does the full entropy dynamics prohibit ∇S = 0 except in a trivial or physically inaccessible sector?

• Can the theory be reformulated so that the metric remains regular even when ∇S vanishes?

I think this is particularly important because ToE treats entropy as ontologically fundamental. A fundamental theory should ideally specify the status of every physically admissible configuration of its fundamental field.

THE WEAK-GRADIENT LIMIT DESERVES A VERY EXPLICIT DERIVATION

Letter III states that the Einstein–Hilbert action emerges from the Obidi Action in the near-equilibrium, weak-gradient, large-scale limit.

This appears to create a subtle mathematical issue that may be worth addressing explicitly.

Since

u_a = ∇_a S / |∇S|,

taking

|∇S| → 0

does not necessarily imply

u_a → 0.

For example, suppose

∇_a S = ε v_a.

Then, for ε ≠ 0,

u_a = v_a / √(G^bc v_b v_c),

which is independent of ε.

Therefore

ε → 0

does not imply

u_a → 0.

Consequently,

G̃_ab = G_ab − 2u_a u_b

does not automatically approach G_ab as |∇S| → 0.

A very simple local counterexample illustrates the issue.

Take

G_ab = δ_ab

and

S = ½ ε (x⁰)².

Then

∇S = ε x⁰ dx⁰,

so for x⁰ ≠ 0,

u_a = ±(1,0,0,0).

Therefore

G̃_ab = diag(−1,+1,+1,+1)

for every nonzero ε.

Letting

ε → 0

makes the entropy gradient arbitrarily small, but the Lorentzian metric does not approach the original Euclidean metric. At x⁰ = 0, meanwhile, ∇S = 0 and the normalized transformation becomes undefined.

I realize that the actual emergence map and coarse-graining construction in ToE may provide the missing mechanism. If so, I think this would be an excellent place to show the complete mathematical chain explicitly:

|∇S| → 0
↓
information-gravity corrections
↓
emergence/coarse-graining map
↓
physical metric g_μν
↓
Einstein–Hilbert sector.

In other words, it would be helpful to demonstrate precisely why the weak-gradient limit gives the physical Einstein metric rather than merely leaving the Lorentzianized metric G̃_ab intact.

THE STATUS OF G_ab, G̃_ab AND THE EMERGENT EINSTEIN METRIC

I think a reader could benefit from an especially explicit distinction between three objects:

(i) the underlying information-geometric metric G_ab,

(ii) the Obidi metric G̃_ab,

(iii) the emergent/coarse-grained physical metric g_μν.

The conceptual chain appears to be something like

information manifold
↓
G_ab
↓
Obidi transformation
↓
G̃_ab
↓
emergence/coarse-graining map
↓
g_μν.

If that is correct, I think the theory would become considerably clearer if this mapping were formalized as a theorem, including the precise assumptions under which

Φ*(G̃) → g

in the infrared limit.

This would also make it much harder for a critic to argue that the Lorentzian structure has simply been inserted at the transformation stage.

THE VARIATIONAL STATUS OF u_a

Another technical point concerns whether u_a is an independent dynamical variable or merely shorthand for the normalized entropy gradient.

If

u_a ≡ ∇_aS / √(G^bc∇_bS∇_cS),

then

G^ab u_a u_b = 1

is already an identity.

But if u_a is treated as an independent field, then the normalization condition must be imposed dynamically, for example with a Lagrange multiplier.

These are not necessarily equivalent variational formulations.

This raises the question:

Is u_a fundamental,
or is u_a entirely derived from S and G?

If it is derived, then when varying the action with respect to G_ab, the variation of u_a must also be included because u_a itself depends on G_ab.

That is,

δu_a ≠ 0

under a general variation δG_ab.

I think an explicit appendix carrying out this full variation would be extremely valuable.

THE FULL VARIATION OF THE OBlDI ACTION

This may be the single most useful mathematical strengthening that could be added to Letter III.

Suppose the total action has the schematic structure

A_gen = A_Obidi[S,G] + A_matter[ψ,G̃] + A_constraint[S,ψ,G,G̃].

Then the metric/information variation should be shown in complete form:

δA_gen/δG_ab = 0.

Because

G̃_cd = G_cd − 2u_cu_d,

and u_c depends on G through its normalization, the variation should contain both the explicit variation of G_cd and the implicit variation through u_c.

A complete derivation from the fundamental action all the way to the claimed Einstein-like equation would, in my opinion, be one of the strongest possible responses to skeptical readers.

The key question is whether the result is genuinely

G_μν + Λ g_μν
= 8πG_eff T_μν + entropic corrections,

as a consequence of the action, or whether some of the Einstein structure has entered through the choice of geometric or constraint terms.

THE MATTER SECTOR

Letter III introduces a standard matter action coupled to the emergent/entropic metric.

That is entirely reasonable as an effective construction.

But I think the theory should carefully distinguish between two different claims:

“matter couples consistently to emergent spacetime”

and

“matter itself is derived from entropy.”

The former can follow from minimal coupling; the latter requires a deeper derivation.

If ToE ultimately claims that matter is emergent from the entropic field, it would be useful to identify exactly where the particle/field degrees of freedom arise and how their action follows from the underlying information dynamics.

Otherwise, the matter sector may reasonably be interpreted as an external sector placed on the emergent geometry.

THE CONSTRAINT SECTOR

Similarly, I would be interested in seeing the constraint action treated with complete variational transparency.

If the constraint action is required to enforce normalization, entropic consistency, or the relationship between the information and physical metrics, that is legitimate.

But the important mathematical question is:

What equations follow from varying every constraint multiplier?

and

What equations follow from varying the fields on which those constraints act?

In particular, if any constraint terms remove higher-derivative contributions or unwanted geometric terms, it would be valuable to show that the coefficients are independently fixed by the underlying principle rather than chosen specifically to produce the Einstein equations.

This distinction would be important for establishing that GR is genuinely a consequence of ToE rather than a structure engineered into it.

## THE EINSTEIN–HILBERT CORRESPONDENCE

I was particularly interested in the statement that the Einstein–Hilbert Action is a limiting/macroscopic image or special case of the Obidi Action.

I think this is potentially one of the strongest claims in the entire theory.

But it would be useful to make the logical status absolutely explicit.

There is a significant difference between:

### (A) the Einstein–Hilbert action can be obtained from the Obidi framework,

and

### (B) the Einstein–Hilbert action is uniquely and necessarily obtained from the fundamental Obidi Action under a mathematically defined limit.

The second is much stronger.

I think a rigorous theorem of the form

Given assumptions A, B, C, ...
the infrared limit of A_Obidi is uniquely
A_EH + suppressed correction terms

would be extremely valuable.

The assumptions should ideally be stated as independently motivated physical or mathematical conditions, rather than simply conditions chosen because they reproduce GR.

## THE VACUUM LIMIT

Another important test seems to be the vacuum sector.

If the complete ToE equations have the schematic form

G_μν + Λ_ent g_μν
= 8πG_eff
[T_μν^(m) + T_μν^(S) + T_μν^(constraint)]
+ corrections,

then setting

T_μν^(m) = 0

does not automatically give ordinary GR vacuum.

The decisive question is whether the remaining entropy and constraint sectors necessarily vanish in a legitimate vacuum solution.

In particular:

Does ToE admit a solution corresponding exactly to

G_μν = 0

in the appropriate vacuum limit?

If not, that would be a genuine physical distinction from vacuum GR.

If yes, I think it would be very useful to exhibit the exact solution and the assumptions under which

T_μν^(S) → 0,

T_μν^(constraint) → 0,

and

Λ_ent → 0

(or whatever precise relation ToE predicts).

## INFORMATION-GEOMETRIC UNIQUENESS

I also think the discussion of **Fisher–Rao geometry** and **Čencov invariance** could be strengthened by distinguishing two propositions.

The **first** is:

**Fisher–Rao geometry by itself is positive definite
and therefore is not already physical Lorentzian spacetime.**

That seems clear.

But the **second proposition,**

**therefore the Obidi Transformation is the uniquely
correct way to obtain physical Lorentzian geometry,**

**requires additional justification.**

There are potentially many ways of extending or deforming a positive-definite information metric.

So it may be useful to formulate a uniqueness theorem:

Under assumptions A, B, C, ...
the only covariant entropy-gradient deformation that
produces a Lorentzian metric while satisfying the
required information-geometric principles is the
Obidi Transformation.

If such a theorem can be established, it would answer one of the most obvious objections immediately.

## THE SPEED OF LIGHT

The same standard of rigor could be applied to the derivation of c.

If

c_ent = √(κ/ρ_S),

then the crucial question is whether κ and ρ_S are themselves independently derived quantities.

A prediction of c requires that neither parameter has effectively been calibrated using the measured value of c.

The strongest possible presentation would therefore trace

fundamental constants
↓
κ and ρ_S
↓
c_ent
↓
measured c

without using c as an input anywhere in the chain.

The same principle applies to G_eff, Λ_ent and other physical constants.

## DIMENSIONAL ANALYSIS AND PARAMETER COUNTING

I think a very useful addition to the ToE programme would be a complete table containing every independent dimensional constant and dimensionless coupling in the theory, specifying:

• where each originates;
• whether it is derived or postulated;
• whether it is free or fixed;
• whether it is experimentally calibrated;
• whether ToE predicts its numerical value;
• whether it disappears in the classical limit.

This would immediately distinguish genuinely predictive relations from parameter redefinitions.

## NOVEL PREDICTIONS

Finally, I think this may ultimately be the most important issue for scientific acceptance.

If ToE reproduces GR exactly in the classical limit, then the theory becomes scientifically distinguishable from GR only through deviations such as

ΔR,
ΔG_μν,
K_Ω,
non-adiabatic entropy corrections,
quantum/information-geometric corrections,
or other measurable residual terms.

It would therefore be extremely valuable to identify a small number of explicit quantitative predictions of the form

Observable_ToE

Observable_GR + Δ(ToE),

where Δ(ToE) is calculable before the experiment is performed.

Even better would be a regime in which

Δ(ToE) ≠ 0

but

Δ(ToE) → 0

in the established classical/GR limit.

That would give the scientific community something very concrete to test.

## A POSSIBLE “MATHEMATICAL RIGOR” APPENDIX

If I may make one constructive suggestion, perhaps future versions of the ToE papers could include a dedicated technical appendix containing, in one uninterrupted chain:

Definition of the fundamental manifold;

Definition of S;

Definition of G_ab;

Definition of u_a;

Derivation of the Obidi Transformation;

Proof of Lorentzian signature;

Treatment of ∇S = 0;

Full variation of the action;

Derivation of every stress-energy contribution;

Derivation of the Einstein-limit action;

Derivation of the Einstein field equations;

Exact assumptions required for the limiting procedure;

Derivation of G_eff and Λ_ent;

Derivation of c;

Explicit novel experimental predictions.

Such an appendix would allow a mathematical physicist to verify the theory without having to reconstruct the derivation from several different conceptual sections.

## MY OVERALL IMPRESSION

I want to emphasize that these questions do not diminish what I find interesting about ToE.

The underlying idea is ambitious: rather than taking spacetime geometry as fundamental, you are attempting to construct a deeper hierarchy

entropy/information
↓
information geometry
↓
physical geometry
↓
gravitation
↓
matter and quantum phenomena.

What I am trying to understand is precisely where each arrow in that chain is a theorem, where it is a postulate, where it is an effective approximation, and where it remains a conjecture.

I think this distinction could actually strengthen the presentation of ToE considerably.

In particular, if the objections above have already been solved elsewhere in the ToE literature, then explicitly bringing those solutions into Letter III would prevent readers from mistaking an already-solved problem for an unresolved one.

And if some of them have not yet been solved, I believe stating them openly as current mathematical problems could also strengthen the programme. A theory does not become weaker by identifying the exact point at which further mathematics is required; in many cases, doing so makes the research programme much more compelling.

I am sending this in the spirit of constructive scrutiny rather than opposition. I am genuinely interested in seeing whether ToE can be developed to the point where a mathematically trained reader can independently follow every step from the fundamental entropic field to Lorentzian spacetime, Einstein gravity, matter, and ultimately the theory’s distinctive experimental predictions.

Thank you for taking the time to read this. I would be very interested in your response to these points, especially if some of the apparent difficulties arise from my incomplete understanding of the formalism.

With warm regards,

**Daniel Moses Alemoh**
