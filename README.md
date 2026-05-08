# SIO Conceptual Framework

> **License:** This work is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
> Attribution required. No commercial use. No derivatives.
> See [LICENSE](./LICENSE) file.

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

**First public commit:** March 27, 2026  
**Last updated:** May 7, 2026  
**Author:** Mélanie Maquet

---

This document defines the core conceptual system underlying Signal Inference Optimization (SIO).

It formalizes how signals degrade, how probabilistic systems reconstruct meaning, and how structured intervention can stabilize interpretation.

---

## 1. Signal Pathologies

Signal degradation follows identifiable patterns:

- **Semantic obesity** — excessive accumulation of concepts, abstractions, or lexical variations without structure or hierarchy within a textual space, producing noise instead of signal. The response is **semantic sobriety**: one concept per textual space, explicit hierarchy, elimination of unanchored abstractions.

- **Content overload** — volume exceeding an organization's semantic governance capacity, introducing involuntary conceptual variability that fragments the signal across the corpus.

- **Terminological fragmentation** — inconsistent vocabulary breaking semantic continuity across the corpus. Fragmentation originates from three sources:
  - **Team fragmentation** — each department develops its own professional vocabulary
  - **Channel fragmentation** — LinkedIn, website, newsletter, case studies produce distinct registers
  - **Period fragmentation** — sedimentary layers of past terminology coexist with current vocabulary

- **Semantic debt** — cumulative cost of content production without terminological governance. Unlike a discrete error, semantic debt accumulates over time and becomes asymmetrically expensive to correct: publishing correct content afterward does not erase months of sedimented drift. Each ungoverned publication adds competing clusters to the existing corpus, diluting the proprietary signal and reinforcing generic reconstructions.

- **Variance operations** — five semantic transformations that probabilistic systems apply to signals during reconstruction:
  - **Generalization** — the system broadens scope beyond actual identity
  - **Amalgamation** — the system merges the entity with competitors or broader categories
  - **Truncation** — the system retains only part of the positioning
  - **Substitution** — the system replaces proprietary concepts with generic equivalents
  - **Projection** — the system attributes typical category properties to the entity

- **Variance manifestations** — five observable symptoms resulting from variance operations:
  - **Interpretive distortion** — reconstruction diverges from intended meaning
  - **Interpretive divergence** — two systems or two close interactions produce incompatible reconstructions
  - **Response instability** — same system generates different responses to similar queries
  - **Probabilistic amplification** — a minority signal becomes dominant through fragment selection
  - **Signal dilution** — no trajectory dominates, producing vague and generic outputs

- **Interpretive sedimentation** — progressive accumulation of plausible inaccuracy layers that consolidate into the reference version used by probabilistic systems. Sedimentation follows a propagation cycle: corpus → ingestion → erroneous reconstruction → republication → re-ingestion → consolidation.

- **Interpretive diagenesis** — the process by which nascent sedimentation (still reversible at reasonable cost) transforms into consolidated sedimentation (structurally rigid, asymmetrically expensive to correct). The geological metaphor is deliberate: loose sediments become rock.

---

## 2. Spaces and Mechanisms

### Dual space architecture

- **Interpretive space** — the global informational environment in which linguistic signals circulate. Includes all endogenous corpus (controlled by the organization), exogenous corpus with partial control, and exogenous corpus beyond control. This is the signal source — the terrain on which an organization acts.

- **Inference space** — the internal vectorial/probabilistic space of the LLM where embeddings distribute and the model arbitrates between competing trajectories to reconstruct a response. This is the signal processing — the terrain the organization cannot control, only influence.

The distinction is foundational:  
You govern the interpretive space.  
The model operates in the inference space.  
Inference drift is the gap between the two.

### Mechanisms

- **Probabilistic compression** — transformation of information into statistical representations with inherent loss. Operates as a filter that retains statistically dominant regularities and eliminates the rest, regardless of quality or intent.

- **Fragmentary autonomy** — independent reconstruction of partial signals without global coherence guarantees. The fragment is the unit of meaning for LLMs; the document is the unit of meaning for humans.

- **Probabilistic reconstruction** — generation of meaning from compressed distributions rather than direct retrieval. Reconstruction is inference, not description. It produces the most probable version, not the most accurate version.

- **Inference pipeline** — sequence of transformations shaping output. Two modes exist:

### Single-hop pipeline

  1. **Query analysis** — intent, entities, freshness assessment. The model decides whether to search the web.
  2. **Query expansion** — the query is reformulated with lexical variants, synonyms, and associated terms. The search surface extends beyond the original wording.
  3. **Web search** — lexical relevance, domain authority, freshness. This is where SEO remains necessary. It conditions entry into the pipeline. But entering the pipeline is not surviving it.
  4. **Page selection** — relevant pages are identified and retrieved.
  5. **Extraction and cleaning** — noise removed (navigation, ads, non-informational blocks). Useful content isolated.
  6. **Semantic chunking** — content is split into semantically coherent, ideally autonomous fragments. From this point, the content ceases to exist as a page. It becomes a point in a vectorial space.
  7. **Embedding** — each chunk is transformed into a vector representation of its semantic content.
  8. **Hybrid retrieval** — combines vectorial signals (semantic proximity) and lexical signals (exact term matching). A chunk that covers the right subject but lacks the precise query terms can be discarded in favor of a lexically matching but conceptually weaker competitor.
  9. **Reranking** — optimizes for actual relevance to the question, beyond raw vectorial similarity.
  10. **Context construction** — retained chunks are filtered (redundancy removed), then compressed to fit the model's token limit. Some chunks disappear at this stage.
  11. **Generation** — the model produces its response from this constructed context, not from the site, not from the article, but from the fragments that survived all transformations.

### Multi-hop pipeline

  Complex queries trigger multiple pipelines simultaneously.

  1. **Complexity analysis** — multi-intent detection, dependency mapping.
  2. **Query fan-out** — decomposition into distinct sub-queries.
  3. **Parallel pipelines per sub-query** — each sub-query follows its own full single-hop pipeline: expansion → web search → selection → extraction → chunking → embedding → retrieval → reranking → **local synthesis**.
  4. **Local synthesis** — intermediate synthesis produced for each sub-query before assembly. This is where drift becomes maximal: chunks from different sources using divergent terminology for the same concept produce divergent embeddings that partially cancel each other instead of reinforcing.
  5. **Synthesis fusion** — alignment, deduplication, divergence resolution across local syntheses.
  6. **Global context construction** — final selection and compression.
  7. **Final generation** — response produced from the fused global context.

### Five signal disappearance points

  Signal does not disappear all at once. It dies stage by stage:

  1. **Extraction** — structurally ambiguous content (dense paragraphs, unclear sections, mixed concepts) produces uninterpretable blocks. Everything downstream fails.
  2. **Chunking** — a chunk that depends on previous context to be understood is a dead chunk. The model sees isolated fragments, not your article.
  3. **Retrieval** — each chunk competes directly against chunks from all other selected sources. A semantically weak or terminologically unstable signal loses this competition even if the page was selected by web search.
  4. **Internal non-competition** — chunks from the same corpus compete against each other. A redundant corpus dilutes its own vectorial signal. A corpus can fight against itself and lose.
  5. **Multi-hop synthesis** — presence across multiple sub-queries with divergent terminology does not reinforce. It partially cancels during synthesis. Terminological stability across an entire corpus is not an editorial detail. It is a survival condition.

### Local chunk competition

- **Chunk competition** — operational mechanism by which LLMs select which chunks survive in the final response when multiple chunks describe the same subject. For each query, only a limited subset of chunks is mobilized in the competition window. Within that window, your chunks compete directly against those of other organizations covering the same territory. The competition is local to the query, not global to the sector.

- **Vectorial attractivity** — what makes one chunk preferred over another in the local competition window. Determined by four governable dimensions: semantic coherence (stable terminology, predictable co-occurrences), fragmentary autonomy (chunk understandable in isolation), conceptual precision (explicit distinctive markers), resistance to compression (central concept early, clear hierarchy).

The distinction matters: typicality bias operates at two levels. The global level pulls identity toward the sectoral prototype — accessible only to organizations with massive accumulation. The local level operates in chunk competition windows — accessible to any organization that applies the discipline. Local victory is the operational terrain of SIO.

### Context window

- **Context window** — the token limit a model can process simultaneously during generation. A mechanical constraint that forces compression and selection of signals. When available embeddings exceed the context window capacity, the model must arbitrate aggressively, amplifying variance. This constraint is particularly acute for users of free or lightweight interfaces, where reduced context windows compound compression effects.

---

## 3. Fundamental Laws

### Structural constraints

- Meaning is not retrieved. It is reconstructed.
- Reconstruction is probabilistic, not deterministic.
- Signal degradation is cumulative across the inference pipeline.
- Unstructured signals drift by default.
- What survives reconstruction defines perceived identity.

SIO operates under these constraints.

### The five laws of linguistic engineering

These are not recommendations. They are structural constraints. Violating one weakens the other four. They operate simultaneously, not sequentially.

- **Law of density** — a signal exists only if it reaches the statistical threshold sufficient to form an interpretive cluster in the inference space.
- **Law of coherence** — the same realities must be designated by the same terms, in the same conceptual associations, across all channels, teams, and periods.
- **Law of hierarchy** — not all signals are equivalent. Pillar content carries the central signal. Peripheral content illustrates and contextualizes. This hierarchy must be intentional.
- **Law of fragmentary autonomy** — each passage must be able to exist alone, be understood, be relevant, and carry complete information without depending on adjacent passages.
- **Law of freshness** — a static corpus degrades. Signals must be renewed regularly to maintain weight against model update cycles and continuous informational competition.

---

## 4. Informational Identity

- **Probabilistic informational identity** — identity as reconstructed outputs, not retrieved facts. A statistical distribution of possible versions of an entity, never directly accessible, only observable through sampling.
- **Informational dominance** — relative influence of a signal within competing reconstruction candidates. Rests on four dimensions: density, coherence, repetition, freshness.
  - **Offensive dominance** — deliberate construction of dominant signals through oriented production, canonical structuring, and multi-source distribution.
  - **Defensive dominance** — preservation of constructed dominance through inference audit and continuous semantic monitoring.
- **Informational corpus** — total available signal contributing to reconstruction, structured in three zones:
  - **Endogenous corpus** — internally controlled signal production (site, declarative signal files, institutional documents)
  - **Exogenous corpus with partial control** — off-site signals with influence but not final control (LinkedIn, interviews, solicited press, aligned partners)
  - **Exogenous corpus beyond control** — signals neither produced nor modifiable (forums, Reddit, third-party comparisons, unsolicited press)
- **Signal** — structured informational input entering probabilistic systems. The primary unit of influence in probabilistic reconstruction.

Informational identity cannot be controlled directly.  
It can only be influenced through signal structuring.

It emerges from the interaction between signals and probabilistic systems.

---

## 5. Methodological Foundations

### Three levels of engineering

- **Corpus engineering** (macro level) — global architecture of all content: volume, hierarchy, multi-source coherence, systemic consistency. Prevents fragmentation at scale.
- **Semantic engineering** (intermediate level) — structure of meaning within the corpus: relationships between concepts, conceptual hierarchies, intentional associations. Maintains coherence within thematic domains.
- **Linguistic engineering** (micro level) — deliberate choice of words and terms, terminological stability, Codebook application, semantic sobriety. The execution layer.

### Core tools

- **Semantic Codebook** — the central governance infrastructure structuring how an organization codes its canonical concepts, terms, obligatory associations, and excluded formulations to produce a stable signal readable by AI systems. Structure: canonical term → definition → admitted synonyms → excluded formulations → obligatory associations → coherence note. See dedicated document: [codebook.md](https://github.com/MMaquet/signal-inference-optimization/blob/main/codebook.md).

- **Governed Writing Protocol** — the methodological framework that produces content surviving the inference pipeline. The Protocol operationalizes the five laws of linguistic engineering through three structural rules applied to every content unit:
  - **Semantic autonomy** — each passage must be extractable from its context and remain comprehensible. No orphan pronouns, no internal references requiring prior context.
  - **Conceptual density** — each passage must contain the canonical term of the concept it develops. No periphrasis, no metaphorical replacement.
  - **Terminological coherence** — one dominant concept per unit, anchored in the corpus signal.
  
  The Protocol produces Autonomous Inference Units. It is the bridge between the Semantic Codebook (which terms) and corpus deployment (how those terms travel through the pipeline).

- **Autonomous Inference Unit (AIU)** — paragraph or content block containing complete signal independently, designed to survive chunking with its proprietary terminology intact. An AIU does not depend on other paragraphs to be understood, contains no orphan pronouns, and carries the canonical term of the concept it develops. The AIU is the smallest content unit on which the Governed Writing Protocol applies. The unit name reads: a block (Unit) constructed for the model's reconstruction process (Inference) that carries its meaning independently of its origin context (Autonomous).

- **Interpretive orchestration** — the technical infrastructure that makes canonical corpus signals explicitly accessible and amplified for AI systems. Encompasses machine-readable files that declare and amplify existing signal:
  - **Declarative layer**: signal-identity.json, signal-claims.json, inference-corrections.json, signal-manifest.json, signal-policy.json, signal-context.txt, llms.txt, llms-full.txt, humans.txt, JSON-LD, Schema.org
  - **Thematic corpus layer**: structured Markdown files, one per key domain, optimized for retrieval by RAG systems

- **Semantic sobriety** — editorial discipline opposing semantic obesity. One concept per textual space, explicit hierarchization, elimination of unanchored abstractions, Codebook compliance.

- **Proprietary conceptual core** — controlled semantic structure designed to resist compression and guide reconstruction. Non-synonymizable. Non-negotiable.

- **Core/Periphery architecture** — structural distribution of terminology within content, organizing the relationship between proprietary terms and market terms:
  - **Core** — proprietary terms from the Semantic Codebook. Occupy dominant positions: titles, opening paragraphs, definitions, repeated conceptual anchors. The core is what the model retains under compression.
  - **Periphery** — market terms (industry vocabulary, common search terms). Occupy secondary positions: contextual illustrations, accessibility bridges, lexical enrichment. The periphery is what enables retrieval entry, never what defines reconstruction.
  
  Market terms enter the pipeline. Proprietary terms survive inside it. Core/Periphery architecture is the structural answer to the SEO/SIO articulation: SEO needs market terms in periphery for retrieval; SIO needs proprietary terms in core for fidelity.

- **Content hierarchy** — structured distribution of information to reinforce dominance. Pillar content concentrates density; satellite content reinforces without diluting.

- **Corpus architecture** — global organization of content ensuring consistency and density across the three corpus zones.

- **Declarative signal files** — machine-readable files that declare and amplify canonical signals in machine-native formats. These files densify the identity signal without commanding the model. They compete as chunks in the pipeline and win by density when properly structured.

- **Inference audit** — systematic multi-model, multi-run, multi-angle interrogation of LLMs to extract the machine thesaurus. The audit measures what probabilistic systems actually reconstruct from a corpus. Method: same entity queried across ChatGPT, Perplexity, Gemini, with multiple runs per query, multiple query angles per entity, comparison against projected and expressed thesauri. The audit identifies which variance operation is dominant, where in the pipeline signal dies, and which corrective intervention is structurally appropriate.

- **Typed correction** — diagnostic-driven intervention adapted to the specific variance operation identified. Generic correction in a probabilistic system is random correction. Typed correction matches intervention to cause:
  - **Generalization** → densify the central concept, rebalance core/periphery ratio
  - **Amalgamation** → reinforce proprietary concepts, exclude shared terms from the core
  - **Truncation** → strengthen obligatory co-occurrences between concept components
  - **Substitution** → exclude generic equivalent, densify proprietary term, create contrastive associations
  - **Projection** → saturate real signal, declare exclusions in machine-readable files (inference-corrections.json), avoid editorial negation
  
  Priority order: loss → distortion → pollution. Loss of identity (amalgamation, substitution) treats first because no other correction has effect without identity. Distortion (generalization) treats second. Incomplete signal (truncation) treats third. Polluted signal (projection) treats last.

### The rule of three autonomies

Structural framework ensuring content survives LLM fragmentation at every scale:

- **Fragment autonomy** — each passage contains its central concept explicitly named, understandable without surrounding context.
- **Page autonomy** — each article carries one dominant concept; others illustrate it without competing.
- **Corpus autonomy** — each concept is designated by a stable, unique term across all channels and periods.

---

## 6. Discipline

- **Informational ecology** — management of signal environments and interactions. Three dimensions:
  - **Sectoral semantic monitoring** — mapping the ecosystem in which the corpus exists
  - **Corpus discipline** — maintaining internal coherence and terminological stability
  - **Inference audit** — systematic multi-model, multi-run interrogation to measure what systems reconstruct, detect drift, and intervene before sedimentation consolidates

- **Interpretable web** — web structured for probabilistic interpretation rather than indexing. Publishing to be reconstructed, not to be visited. The site as interpretive tool, not showcase.

- **Consensus engineering** — deliberate shaping of shared interpretations through structured signal. The result of Codebook + five laws + interpretive orchestration + corpus architecture + informational ecology applied together. Four conditions: abandonment of parasitic terms, proprietary conceptual core, mastered repetition over time, signal hierarchy. Four measurement signals: inter-contextual stability, reformulation resistance, multi-query coherence, semantic convergence.

- **Attractive density** — capacity of a dense, coherent signal to dominate reconstruction through mass and coherence. The vectorial mechanism that produces the interpretive center of gravity. Attractive density is the engine; the center of gravity is the observable result.

---

## 7. Limits and Risks

- **Semantic contamination** — deliberate construction of signals disconnected from actual reality. Distinct from AI poisoning (external attack): contamination is a practitioner building a fictional signal for their client.

- **Manipulation vs governance** — boundary between structuring a truthful signal and fabricating a misleading one. Objective criterion: correspondence to defensible reality. Subjective criterion: intent.

- **Stability of interpretive center of gravity** — ability of a structured signal in the interpretive space to resist drift over time against competing exogenous signals.

- **Stability of inference center of gravity** — ability of the reconstructed representation in the inference space to remain consistent across contexts, models, and time.

- **Training bias** — inherited distortions from underlying model training data. A structural limit that corpus engineering alone cannot neutralize.

- **Asymmetric correction** — correcting consolidated sedimentation requires the correct signal to be simultaneously dominant, coherent, and repeated over time. Publishing correct content does not erase sedimentary layers.

---

## 8. Core SIO Concepts

- **Signal Inference Optimization (SIO)** — the discipline of structuring the signal made available to probabilistic systems in order to reduce inference drift and orient LLM reconstructions toward a version faithful to intended meaning. SIO does not optimize inference. It optimizes the signal that enters the inference process. The name reads: optimization of the signal *for* inference — not optimization *of* inference itself. SIO is the discipline of signal resilience through a destructive pipeline.

- **Interpretive center of gravity** — the dominant cluster in the interpretive space. The source signal sufficiently dense and coherent to orient reconstructions toward a chosen version. This is what you build.

- **Inference center of gravity** — the convergence point toward which embeddings and probabilistic trajectories converge in the inference space. The observable effect of the reconstruction produced by the model. This is what you measure.

- **Stable reconstruction** — consistent output across contexts and probabilistic variations.

- **Inference drift** — deviation between intended meaning and reconstructed output. The gap between interpretive space (what you inject) and inference space (what the model produces).

- **Semantic mass** — weight of a concept determined by density, coherence, and repetition. Semantic mass determines whether a signal survives probabilistic compression.

- **Attractive density** — capacity of a dense, coherent endogenous corpus to reduce the relative weight of uncontrolled exogenous signals in LLM reconstruction. The underlying vectorial mechanism that produces the interpretive center of gravity.

- **Probabilistic governance** — the posture of governing signal inputs to influence reconstruction outputs, with full acknowledgment that correlation is observable but causality is not provable. Not control. Influence under structural uncertainty.

- **Variance operations vs variance manifestations** — analytical distinction between the underlying transformations applied by probabilistic systems (operations: generalization, amalgamation, truncation, substitution, projection) and their observable symptoms in reconstructions (manifestations: distortion, divergence, instability, amplification, dilution). The distinction matters diagnostically: manifestations are what the audit observes; operations are what corrective intervention must address. Treating manifestations without identifying operations produces generic correction, which in a probabilistic system equals random correction.

- **Diagnostic methodology cycle** — the operational sequence: diagnostic → codebook → inference audit → corrective → re-audit. The cycle is not linear but iterative. Each re-audit informs the next diagnostic. The Codebook evolves with the corpus. The audit recalibrates with model updates and corpus growth.

---

## 9. Diagnostic Methodology

The three-thesaurus framework defines the diagnostic foundation of SIO practice.

It measures the gap between what an organization believes it signals, what it actually signals, and what probabilistic systems reconstruct from that signal.

### Thesaurus layers

- **Projected thesaurus** — the conceptual vocabulary an organization believes it is communicating. Reflects strategic intent and self-perception.
- **Expressed thesaurus** — the conceptual vocabulary actually present in the informational corpus, both endogenous and controlled exogenous. Reflects what is genuinely available to probabilistic systems for reconstruction.
- **Machine thesaurus** — the conceptual vocabulary effectively reconstructed by LLMs, extracted through systematic multi-model, multi-run interrogation.

### Diagnostic gaps

- Gap between projected and expressed thesaurus reveals internal incoherence — editorial drift, terminological fragmentation, or misalignment between intent and production.

- Gap between expressed and machine thesaurus reveals signal failure — inference drift, chunking loss, or dilution through retrieval and reconstruction.

- The projected thesaurus is never compared directly to the machine thesaurus. The expressed corpus is the only observable and actionable terrain.

### Service sequence

diagnostic → codebook → inference audit → corrective → re-audit

### Foundational principle

The objective is not measurement for its own sake. It is corrective.

The goal is to ensure that the concepts, relationships, and meaning present in the projected and expressed thesaurus survive the inference pipeline — chunking, embedding, retrieval, reranking, and generation — and emerge intact in the machine thesaurus.

Signal structure is not sufficient.  
Signal survival through transformation is the standard.

---

## Status

This framework is evolving and will be refined through:

- applied methodologies
- inference audits
- real-world implementations

---

## License

This document is licensed under the Creative Commons 
Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0).

You may share this work with attribution.  
You may not use it commercially.  
You may not modify or redistribute modified versions.

Full license text: https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode  
See [LICENSE](./LICENSE) file in this repository.

For commercial licensing, derivative works, or formal collaboration:  
[Mélanie Maquet on LinkedIn](https://www.linkedin.com/in/melaniemaquet/)

---

## Reference

This document is part of the Signal Inference Optimization (SIO) conceptual framework:

- [SIO README](https://github.com/MMaquet/signal-inference-optimization/blob/main/README.md)
- [Semantic Codebook](https://github.com/MMaquet/signal-inference-optimization/blob/main/codebook.md)
- [Article series](https://medium.com/@melaniemaquet)

**First public commit:** March 27, 2026  
**Last updated:** May 7, 2026  
**Author:** Mélanie Maquet — SEMANTIKIA
