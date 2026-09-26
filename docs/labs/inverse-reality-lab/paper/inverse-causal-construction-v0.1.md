---
title: "Inverse Causal Construction"
subtitle: "A Chrono-Topological Framework for Reconstructing Monumental Building Sequences from Terminal Physical States"
author:
  - "Deep Analytica Research"
date: "26 September 2026"
abstract: |
  This working paper proposes Inverse Causal Construction (ICC), a framework for reconstructing families of physically and archaeologically compatible construction histories from a finished object's terminal state. Rather than selecting a preferred historical narrative and simulating it forward, ICC begins with measurable geometry, materials, lithology, internal voids, load paths, provenance, archaeological evidence and uncertainty, then infers predecessor states under explicit constraints. The Great Pyramid of Khufu is used as the principal test case. The framework introduces separate positive-material and negative-topological representations, local temporal fields rather than a single height-as-time coordinate, a multi-relation dependency graph, signed bookkeeping for inverse mass removal and gravitational-potential release, and counterfactual falsification in which each historical hypothesis must predict observable traces. Vaidya collapse and Kerr null-geodesic accessibility are used only as cross-domain mathematical laboratories for accessibility topology; they are not proposed as mechanisms of pyramid construction.
keywords:
  - Egyptology
  - computational Egyptology
  - Great Pyramid of Giza
  - Khufu
  - computational archaeology
  - inverse problems
  - construction sequencing
  - 4D reconstruction
  - muography
  - persistent homology
  - Bayesian archaeology
---

# Research question

The terminal monument is observable while the complete construction sequence is not. Direct evidence nevertheless survives across several domains: the major quarry south of the Great Pyramid and extraction traces; the Wadi el-Jarf papyri documenting Inspector Merer's transport of Tura limestone toward Akhet-Khufu [@Tallet2017]; modern material characterization [@Sessa2026; @Hemeda2020]; muographic detections including the ScanPyramids Big Void and North Face Corridor [@Morishima2017; @Procureur2023]; geomorphology [@Kawae2011]; and paleohydrological reconstruction [@Ghoneim2024].

ICC replaces the question *"Which construction method was used?"* with:

$$
\boxed{P(\Gamma,D,C\mid Y,\mathcal{L},E)}
$$

where $\Gamma$ is a construction history, $D$ a design state, $C$ a conception state, $Y$ measurable evidence, $\mathcal{L}$ physical and mathematical constraints, and $E$ archaeological context.

The scientific objective is not to force one story. It is to eliminate histories that are physically impossible, unscalable, archaeologically incompatible, contradicted by observations, or fundamentally non-identifiable.

# Two inverse problems

The present monument is not identical to the monument at completion. Weathering, salt transport, fracture growth, casing removal, later intrusions, earthquakes and conservation interventions altered it.

We therefore distinguish:

$$
C\rightarrow D\rightarrow\Gamma\rightarrow X_F\rightarrow X_N\rightarrow Y_N
$$

where $X_F$ is the completed as-built state, $X_N$ the present physical state and $Y_N$ today's observations.

The full inverse program is:

$$
\boxed{Y_N\rightarrow X_N\rightarrow X_F\rightarrow\Gamma\rightarrow D\rightarrow C}
$$

The first inversion reconstructs the original completed state from the altered present monument. The second reconstructs construction itself.

A generic observation equation is:

$$
Y_N=
\mathcal{O}
\left[
\mathcal{D}_{post}
\left(
\mathcal{B}(C,D,\Theta_B),\Theta_P
\right)
\right]
+\varepsilon
$$

where $\mathcal{B}$ is the construction operator, $\mathcal{D}_{post}$ post-construction transformation, $\mathcal{O}$ observation and $\varepsilon$ measurement error.

# Terminal-state ontology

A terminal state cannot be represented only by height, volume and block count. We define:

$$
X(t)=
\left[
G,L,M,S,F,V,I,A,H,Q,D_g,\mathcal{C},\mathcal{E}
\right]_t
$$

with:

- $G$: external and internal geometry;
- $L$: lithology;
- $M$: density, porosity, elastic and frictional material fields;
- $S$: bedrock/substrate;
- $F$: fractures and discontinuities;
- $V$: known and unknown voids;
- $I$: material interfaces and contacts;
- $A$: architecture;
- $H$: hydrological and landscape state;
- $Q$: material provenance;
- $D_g$: load paths and gravitational support;
- $\mathcal{C}$: causal/dependency relations;
- $\mathcal{E}$: traceable evidence references.

The ontology explicitly distinguishes **observed**, **derived**, **necessary**, **supported**, **plausible**, **speculative**, **unknown** and **contradicted** claims.

# Local chronology: height is not time

A single global height coordinate cannot represent simultaneous work fronts, storage platforms, internal structures, trenches or temporary works.

We therefore replace "height at time $t$" with a local construction surface:

$$
\boxed{h(x,y,t)}
$$

For material position $\mathbf{x}$ define:

$$
\tau_M(\mathbf{x})
=
\text{inferred incorporation time of material at }\mathbf{x}
$$

and for an intentional void:

$$
\tau_V(\mathbf{x})
=
\text{inferred time at which }\mathbf{x}\text{ became constrained to remain unoccupied}
$$

A chamber can therefore have several distinct births:

1. spatial reservation;
2. lower-boundary formation;
3. wall growth;
4. closure;
5. structural completion;
6. encapsulation.

This is central to the King's Chamber prototype: reaching its geometric elevation in reverse is not sufficient to erase it. Its later dependent structure must first become removable.

# Positive matter and negative topological objects

Let $D$ be a design domain and $M(t)\subset D$ the subset occupied by construction material. Its complement is:

$$
V(t)=D\setminus M(t)
$$

Not every empty region is architectural. Outside air, temporary clearances, passages and intentional enclosed spaces have different semantics. ICC therefore treats selected subsets of $V(t)$ as **negative topological objects**.

For chamber $C$ with target boundary $\partial C$, define boundary completion:

$$
\boxed{
\eta_C(t)=
\frac{
\operatorname{Area}(\partial C\cap M(t))
}{
\operatorname{Area}(\partial C)
}
}
$$

A chamber may cease to exist as an architectural object before its Euclidean region disappears: once the enclosing boundary opens sufficiently, the region merges with exterior construction space.

A useful reference-solid bookkeeping quantity is:

$$
\boxed{
m_C^{\ominus}
=
-\int_C \rho_{ref}(\mathbf{x})\,dV
}
$$

This is a **counterfactual absent-mass equivalent**. It is not physical negative mass and creates no antigravity.

# Geometry, inverse mass and gravitational energy

For an ideal square pyramid of base side $a$ and height $H$:

$$
A(z)=a^2\left(1-\frac{z}{H}\right)^2
$$

and:

$$
V=\frac{a^2H}{3}
$$

If a geometric inverse dismantling leaves height $z=uH$, the removed upper-volume fraction is:

$$
\boxed{\Gamma_M=(1-u)^3}
$$

For uniform density, gravitational potential energy relative to the base is proportional to $\int zA(z)dz$. The fraction stored in the removed upper portion is:

$$
\boxed{
\Gamma_G=
1-6u^2+8u^3-3u^4
}
$$

Thus height, removed mass and released potential energy are three different clocks.

Define inferential reverse time:

$$
\tau=T-t
$$

so that:

$$
\frac{d}{d\tau}=-\frac{d}{dt}
$$

but the acceleration due to gravity does not reverse. Along an exactly reversed elevation trajectory:

$$
\boxed{
\Delta U_g^{-}=-\Delta U_g^{+}
}
$$

Likewise inverse mass removal is signed bookkeeping:

$$
dm^{-}=-dm^{+}
$$

while all physical stone masses remain positive.

# Dependency multigraph

Construction is represented as a directed multigraph:

$$
\mathcal{G}=(V,E_C,E_G,E_A,E_V,E_L)
$$

where edges encode:

- $E_C$: construction precedence;
- $E_G$: geometric prerequisites;
- $E_A$: access dependencies;
- $E_V$: void-preservation dependencies;
- $E_L$: gravitational/load-path dependencies.

The effective partial order is the transitive closure of these relations.

An element is eligible for inverse removal only if it is maximal under the active order and passes physical gates:

$$
\boxed{
\mathcal{A}^{-}(X)
=
\left\{
e:
\deg_{\prec}^{+}(e)=0,
\;Stable(X-e),
\;Accessible(e)
\right\}
}
$$

This replaces naive layer-by-layer deletion.

# King's Chamber as first inverse subproblem

The King's Chamber combines an intentional negative volume, granite surfaces, a vertically stacked relieving superstructure, connections to the Grand Gallery/Antechamber system and substantial overlying masonry.

Recent material characterization reports chamber dimensions of approximately 10.5 m by 5.2 m by 5.8 m and distinguishes its red Aswan granite surfaces from the limestone Queen's Chamber [@Sessa2026].

A candidate inverse state path is:

> encapsulated → exposed superstructure → closed chamber → open-top negative object → partially bounded reserved volume → undifferentiated construction space

The exact sequence and timing are not assumed. They must emerge from geometry, dependencies, stability, access and evidence.

The next version should construct an element-level DAG for:

- chamber floor;
- wall courses;
- ceiling beams;
- the stacked relieving spaces;
- upper gabled elements;
- antechamber;
- Grand Gallery connections;
- shafts;
- surrounding masonry.

# Topology and persistence

Let $\mathcal{K}^{+}$ denote a cell complex of material and $\mathcal{K}^{-}$ a semantically classified negative-space complex.

The topology of voids can be studied through:

$$
H_k(V)
$$

and, relative to exterior space $E_{out}$:

$$
H_k(V,E_{out})
$$

Persistent topology can record birth/death events of chambers, corridors and connections during candidate inverse sequences. Two historical hypotheses with similar terminal geometry may therefore predict different topological genealogies.

# Logistics and scalability

A mechanism that can move one block does not automatically scale to a monument.

For a logistics network with edge flows $f_e(t)$ and capacities $c_e(t)$:

$$
0\le f_e(t)\le c_e(t)
$$

and intermediate nodes require mass/inventory balance.

Candidate histories should also satisfy:

- labor capacity;
- transport throughput;
- storage/buffer capacity;
- temporary works;
- simultaneous work-front access;
- quarry production;
- water/river transport constraints where applicable.

ICC therefore distinguishes:

> possible → feasible → scalable → historically compatible

# Bayesian non-identifiability

Several histories may produce terminal states indistinguishable under available evidence.

For latent history/state $Z$:

$$
\boxed{
P(Z\mid Y)
\propto
P(Y\mid Z)P(Z)
}
$$

If two candidate histories remain observationally indistinguishable, the correct scientific answer is **non-identifiability**, not a fabricated unique story.

# Counterfactual falsification

Each historical hypothesis $H$ must predict evidence:

$$
\widehat{Y}_H=\mathcal{C}(H)
$$

The prediction is compared with observation by likelihood or discrepancy:

$$
P(Y_{obs}\mid H)
$$

or:

$$
d(H)=d(Y_{obs},\widehat{Y}_H)
$$

Examples of predicted traces may include:

- muographic density patterns;
- structural contact/load signatures;
- material-provenance distributions;
- course/block-size changes;
- quarry-volume requirements;
- access geometries;
- surviving temporary-work traces.

This is the key step from historical plausibility to falsifiable inverse science.

# Cross-domain accessibility laboratory

Vaidya and Kerr are included only to stress-test mathematics of accessibility boundaries. They are **not mechanisms of pyramid construction**.

A general relation-defined complement is:

$$
\boxed{
N_{\mathcal{R}}(\lambda)
=
\Omega
\setminus
Accessible_{\mathcal{R}}(\Omega,\lambda)
}
$$

The relation $\mathcal{R}$ can mean:

- material/architectural accessibility;
- causal escape accessibility;
- phase-space/geodesic accessibility.

## Vaidya

For a spherical ingoing Vaidya model:

$$
ds^2=
-\left(1-\frac{2m(v)}{r}\right)dv^2
+2\,dv\,dr
+r^2d\Omega^2
$$

the laboratory tracks a local apparent-horizon proxy near $r=2m(v)$ and compares it with a globally integrated outgoing-null boundary. This illustrates why global causal structure cannot always be inferred from a purely local state.

## Kerr

For equatorial null geodesics with Carter constant $Q=0$:

$$
R(r;b)
=
[r^2+a^2-ab]^2
-
\Delta(b-a)^2
$$

with:

$$
\Delta=r^2-2Mr+a^2
$$

Allowed radii satisfy $R\ge0$. At a light-ring separatrix:

$$
\boxed{
R=0,
\qquad
\frac{\partial R}{\partial r}=0
}
$$

The double root can coincide with a change in the number of connected radial-accessibility components.

These examples suggest an abstract critical-boundary condition:

$$
\boxed{
\Phi(x;\lambda)=0,
\qquad
\nabla_x\Phi(x;\lambda)=0
}
$$

Again, this is a mathematical analogy about accessibility topology.

# Evidence anchors

The current release is anchored by traceable external evidence:

- Cosmic-ray muography of the Big Void [@Morishima2017].
- Muographic characterization of the North Face Corridor [@Procureur2023].
- Material characterization of the King's and Queen's Chambers [@Sessa2026].
- Published discussion of Giza stone/material deterioration and engineering properties [@Hemeda2020].
- Giza Plateau geomorphology [@Kawae2011].
- The Ahramat paleochannel reconstruction [@Ghoneim2024].
- Merer's Wadi el-Jarf logbook and Tura limestone transport [@Tallet2017].
- The Great Pyramid quarry and extraction traces documented by Ancient Egypt Research Associates [@AERAQuarry].
- Kerr light-ring topology as mathematical background for the cross-domain accessibility laboratory [@Cunha2020].
- Relativistic singularity/horizon distinctions [@Landsman2021; @Kunduri2013].

# What is established and what is proposed

**Externally supported inputs** include the monument, measured geometry, archaeological context, material studies, quarry evidence, textual transport evidence, muographic detections and landscape/hydrological research.

**Proposed research constructs** include:

- Inverse Causal Construction as an integrated framework;
- the Inverse Reality Ontology;
- negative-topological construction objects;
- counterfactual absent-mass equivalents;
- local material/void birth-time fields;
- the multi-order dependency graph;
- combined mass-energy-topology inverse coordinates;
- complement-defined accessibility objects as a cross-domain mathematical vocabulary.

This release does **not** claim:

1. that the true pyramid construction sequence has been recovered;
2. that the framework has been peer reviewed;
3. that general relativity explains pyramid construction;
4. that the proposed integration is unprecedented across every adjacent literature.

A formal novelty claim requires systematic review against Harris matrices, Bayesian archaeology, 4D BIM, assembly/disassembly planning, inverse procedural modeling, digital twins, inverse mechanics and topological data analysis.

# Falsifiable research program

The next scientific milestone is an element-level King's Chamber and relieving-system graph built from authoritative survey coordinates.

Priority tasks:

1. ingest traceable 3D chamber, gallery, corridor and relieving-system geometry;
2. represent granite and limestone properties as distributions rather than constants;
3. infer load-path constraints with finite- or discrete-element analysis;
4. calculate persistent topology of negative spaces during inverse sequences;
5. model temporary access and reject inaccessible placements/removals;
6. connect material classes to probabilistic quarry provenance;
7. generate hypothesis-specific muography and NDT predictions;
8. fit chronological partial orders under Bayesian uncertainty;
9. publish surviving alternatives and explicit rejection reasons.

# Conclusion

A finished monument is not only a final arrangement of matter. It is also a frozen network of exclusions, interfaces, load paths, provenance, irreversible choices and partial traces of former accessibility.

ICC therefore asks:

$$
\boxed{
\text{Which predecessor states remain possible after all measurable constraints are applied?}
}
$$

The framework will become scientifically valuable only if it produces new testable predictions and rejects attractive hypotheses when reality disagrees.

# Contact

Research discussion, Egyptological critique, survey-data collaboration and computational-archaeology collaboration are welcome:

**Deep Analytica Research**  
contacto@deepanalytica.cl  
https://deepanalytica.cl/labs/inverse-reality-lab/  
https://github.com/deepanalytica

<!-- build-trigger: 2026-09-26-v0.1-r2 -->
