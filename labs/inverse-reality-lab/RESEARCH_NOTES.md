# Theory note - Inverse Causal Construction (ICC)

## Thesis

A finished monument can be treated as a terminal physical state that preserves partial traces of its own production history. Reconstruction should therefore proceed by **constrained causal inversion**, not by selecting a preferred construction story and animating it forward.

## The four separations

1. Present observed state vs. original completed state.
2. Physical positive matter vs. intentional negative topological spaces.
3. Geometric height vs. construction time.
4. Microscopic time reversal vs. inferential backward reconstruction.

## Key proposition

The terminal state contains constraints on the past through geometry, load paths, contact relations, lithology, material provenance, void topology, access, construction scalability and post-construction alteration.

The output is therefore a family of histories:

`P(history | terminal state, evidence, laws)`

rather than a single narrative.

## King's Chamber prototype

The King's Chamber is useful because it combines:

- a deliberately preserved negative volume;
- granite walls and ceiling elements;
- a vertically stacked relieving superstructure;
- connections to the Grand Gallery/Antechamber system;
- known and measurable material surfaces;
- overlying masonry that must post-date at least parts of the chamber complex.

An inverse model should not delete the chamber when a global height slider reaches the chamber elevation. It should first remove the descendants that are later under the inferred partial order. The chamber passes through distinct inverse states: encapsulated -> exposed superstructure -> closed chamber -> open-top negative space -> partially bounded reserved volume -> undifferentiated exterior construction space.

## Cross-domain relativistic laboratory

Vaidya and Kerr are included as mathematical laboratories for accessibility topology. They are not evidence about Egyptian construction. Their purpose is to test whether a common formal vocabulary can represent changes in reachable regions, boundaries and critical bifurcations across very different physical systems.
# Mathematical notebook - Inverse Causal Construction v0.1

## 1. Terminal-state inverse problem

Forward dynamics:

`X_{t+1} = F(X_t, U_t, E_t)`

Inverse predecessor operator:

`Pre(S) = { x : exists u such that F(x,u) in S }`

The research objective is not a unique history, but a posterior over compatible histories:

`P(Gamma | Y, L, E)`

where `Y` is observed evidence, `L` physical laws/constraints, and `E` contextual archaeological evidence.

## 2. Ideal pyramid geometry

For base side `a` and height `H`, a horizontal cross-section at height z has side:

`a(z) = a(1-z/H)`

and area:

`A(z) = a^2(1-z/H)^2`.

Total volume:

`V = a^2 H / 3`.

If dismantling from the apex leaves height `z = uH`, the removed top-volume fraction is:

`Gamma_M = (1-u)^3`.

For uniform density, gravitational potential energy relative to the base is proportional to:

`Integral_0^H z A(z) dz`.

The fraction of potential energy contained in the removed upper part is:

`Gamma_G = 1 - 6u^2 + 8u^3 - 3u^4`.

Thus removed height, mass and gravitational energy are three different clocks.

## 3. Signed mass bookkeeping

Physical mass remains positive. Inverse construction uses a signed bookkeeping increment:

`dm_inv = -dm_forward`.

An intentional void C can carry a counterfactual absent-mass equivalent:

`m_C^- = - Integral_{V_C} rho_ref(x) dV`.

This is a difference relative to a solid reference, not exotic negative mass.

## 4. Negative topology

Let D be the design domain and M(t) the material subset.

`V(t) = D \ M(t)`

is the complement. Architectural negative objects are semantic/topological subsets of V(t).

For a chamber C with ideal boundary dC, define boundary completion:

`eta_C(t) = Area(dC intersect Material(t)) / Area(dC)`.

A chamber can cease to exist as an architectural object before its Euclidean volume disappears, because once its boundary opens sufficiently it merges with the exterior construction space.

## 5. Partial-order reconstruction

Entities form a directed acyclic graph when edges encode required precedence.

An inverse-removable entity must be maximal in the active partial order and pass additional physical gates.

`A^-(X) = { e : outdegree_prec(e)=0 and Stable(X-e) and Accessible(e) }`.

## 6. Gravitational inverse operator

Gravity does not reverse sign under the inferential time coordinate `tau = T-t`. Instead the inverse trajectory reverses the change in potential energy:

`Delta U_g^- = - Delta U_g^+`.

A useful operator is:

`G^-(X,e) = [Delta U_e^-, load_descendants(e), stability(X-e), extraction_work(e)]`.

## 7. Relativistic analogy: causal complement objects

For a relation R, define a complement object:

`N_R(lambda) = Omega \ Accessible_R(Omega, lambda)`.

Examples explored in the lab:

- Pyramid chamber: accessibility through material boundaries.
- Vaidya trapped region: null escape accessibility.
- Kerr radial geodesics: phase-space accessibility where R(r;b) >= 0.

The analogy is mathematical and ontological, not a claim that pyramid voids obey general relativity.

## 8. Critical topology condition

For a scalar constraint Phi(x;lambda), a change in accessible-region topology often occurs at a critical boundary satisfying:

`Phi = 0` and `grad_x Phi = 0`.

For the Kerr equatorial radial potential, this corresponds to the double-root light-ring separatrix.

## 9. Counterfactual falsification

Each construction hypothesis H must predict evidence:

`Y_hat_H = C(H)`.

Comparison to observation uses a loss or likelihood:

`d(H) = d(Y_observed, Y_hat_H)`

or

`P(Y_observed | H)`.

Hypotheses survive only if they are physically feasible, scalable, chronologically compatible and evidentially supported.
# Inverse Reality Ontology (IRO) - working specification v0.1

## Scope

IRO models a finished physical object as a terminal state from which compatible prior states can be inferred under explicit physical, geometric, topological, archaeological and evidential constraints.

It is **not** a claim that microscopic time reversal occurs in nature. The inverse operator is inferential: it searches for predecessor states that could evolve forward into the observed terminal state.

## Core entity classes

- `Observable`: a measured quantity in the terminal or present state.
- `MaterialEntity`: block, mortar joint, bedrock volume, casing stone, granite beam.
- `NegativeTopologicalObject`: intentionally unoccupied volume such as chamber, corridor, shaft or reserved construction void.
- `Interface`: block-block, block-mortar, block-bedrock or void-boundary relation.
- `Event`: placement, extraction, closure, opening, transport, erosion, removal, restoration.
- `Process`: quarrying, hauling, masonry growth, encapsulation, weathering.
- `Constraint`: gravity, contact, stability, accessibility, geometry, conservation, chronology, evidence.
- `EvidenceRef`: traceable measurement, paper, survey, photograph, muography result or textual source.
- `Hypothesis`: candidate causal history.
- `CounterfactualPrediction`: observable expected if a hypothesis were true.

## Signed dual representation

Physical matter is represented by a positive measure `mu+`. Architectural voids may be represented by a **counterfactual absent-mass equivalent** `mu-`, defined relative to an explicit solid reference model. `mu-` is not negative gravitational mass.

## Time fields

For material position x:

`tau_M(x)` = inferred incorporation time.

For intentional void position x:

`tau_V(x)` = inferred time at which the location became constrained to remain unoccupied.

A room can therefore have several births: reservation, boundary formation, closure, structural completion and encapsulation.

## Dependency relations

- `precedes_causal`
- `supports_gravitationally`
- `requires_access`
- `preserves_void`
- `constrains_geometry`
- `derived_from_source`
- `altered_by_postconstruction_event`

The union and transitive closure of these relations define a partial order over construction states.

## Epistemic states

Every inferred edge/node carries one of:

- OBSERVED
- DERIVED
- NECESSARY
- SUPPORTED
- PLAUSIBLE
- SPECULATIVE
- UNKNOWN
- CONTRADICTED

Probability values may supplement but must never replace these semantic states.
# Methods and reproducibility

## Current lab status

Version 0.1 is a conceptual/numerical prototype. It is designed to expose assumptions rather than hide them.

### Pyramid engine

Uses an idealized square-pyramid envelope and a simplified King's Chamber negative-volume model. The height slider is explicitly a geometric dismantling coordinate, not an inferred historical date. The next phase is element-level reconstruction from published surveys/point clouds and material datasets.

### Vaidya engine

Uses a smooth, dimensionless mass function and integrates an outgoing-null generator backward as a pedagogical event-horizon proxy. It is not a full numerical-relativity simulation.

### Kerr engine

Uses equatorial null geodesics (Carter constant Q=0) and the standard radial potential. The accessible radial set is where R(r;b) >= 0; the light-ring critical point is a double-root separatrix.

## Validation gates planned

- geometry against authoritative survey coordinates;
- lithology/provenance uncertainty;
- finite-element structural stability;
- dynamic construction access and temporary works;
- Bayesian chronological constraints;
- persistent-homology tracking for negative spaces;
- counterfactual predictions against muography/NDT observations.
