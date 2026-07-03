> **License:** This work is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
> See [LICENSE](./LICENSE) file.

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

**Author:** Mélanie Maquet

---

# Changelog

All notable changes to the Signal Inference Optimization (SIO) conceptual framework are documented in this file.

This framework follows a deliberate publication cadence — foundational concepts established first, technical operationalization deployed progressively, field validation conducted before public claims.

---

## 2026-07-03

### Concepts enrichment (concepts.md)
- Added **Acknowledgment of presence** in Section 8 (Core SIO Concepts), positioned between *Inference center of gravity* and *Stable reconstruction*.

### Defined
- **Acknowledgment of presence** as the observable status indicating that the source signal has been detected and displayed as a reference by the probabilistic system in its response, without that display constituting control over the reconstruction produced. Acknowledgment of presence attests visibility; it does not guarantee fidelity.
- The distinction between **passive acknowledgment** (observed on the model's output) and **active signal declaration** (posed by the organization through declarative signal files). The two concepts are complementary but architecturally distinct: one is constated, the other is engineered.

### Positioned
- Acknowledgment of presence as a foundational analytical distinction within SIO practice. Being cited proves the signal was seen, not that it was faithfully reconstructed. The concept dismantles the reflex assumption that citation equates to control over reconstruction — a core misconception separating GEO from SIO.
- The concept as a diagnostic anchor within the three-thesaurus framework: it identifies where the machine thesaurus registers presence without necessarily producing fidelity. Presence and fidelity are two independent measurements, not two names for the same phenomenon.

### Rationale
- Formalized a distinction that was implicit across the doctrinal corpus but not named as a canonical concept. The term makes explicit that citation, visibility, and reference display are observable events — not evidence of reconstruction fidelity.
- Anchored the passive/active axis (acknowledgment of presence / signal declaration) as a structural pair within the framework. This axis clarifies why declarative signal files and inference audit are complementary interventions: one engineers the signal upstream, the other measures the observable status downstream.
- Terminology anteriority verified across three surfaces (Google AI overview, Google Web, Google Scholar) prior to canonical publication. LinkedIn phrase-exact verification pending; term released as canonical based on convergence of the three surfaces.

---

## 2026-06-08

### README enrichment — Operational application and canonical surfaces
- **README**: Added "Operational application" section establishing the explicit and locked distinction between SIO (public conceptual framework) and SEMANTIKIA (operational application for organizations).
- **README**: Enriched "Author" section with three canonical surfaces — canonical identity hub on melaniemaquet.com, doctrinal corpus on sio.melaniemaquet.com, professional reference on LinkedIn.
- **README**: Updated "Writing & research" section. The doctrinal corpus is now referenced through sio.melaniemaquet.com, the canonical entry point on the author's own domain.
- **README**: Updated author attribution at the top of the document to "Mélanie Maquet — SEMANTIKIA".
- **README**: Updated last-updated metadata to 2026-06-08.

### Positioned
- **SIO and SEMANTIKIA** as two distinct levels of the same architecture. The conceptual framework is public, open, dated, under Creative Commons license. The operational application is commercial. This distinction prevents the doctrine from being confused with a product, and the product from being confused with the doctrine.
- **sio.melaniemaquet.com** as the canonical entry point of the SIO doctrinal corpus on the author's own domain. Anchors the corpus surface on the canonical domain while preserving chronological paternity of the underlying article series.
- **melaniemaquet.com/identite-canonique** as the canonical identity hub linking the three territories of the author's intellectual work: SIO doctrine, SEMANTIKIA operational application, and Code Karma symbolic reading of life trajectories.

### Rationale
- Made explicit in the README itself the SIO/SEMANTIKIA distinction that has been operationalized across declarative signal files and identity surfaces since May 2026.
- Anchored the doctrinal corpus on a sub-domain of the canonical domain rather than referring readers to an external publishing platform. The canonical surface is now hosted on the author's own infrastructure while preserving the underlying paternity chain.
- Consolidated the three-surface architecture: GitHub (conceptual structure), sio.melaniemaquet.com (doctrinal corpus), semantikia.com (operational application).

---

## 2026-05-28

### Added
- `declarative-hub.md` — Declarative Hub doctrine page. Defines the Declarative Hub as a preventive infrastructure within SIO architecture: a visible, indexed HTML page that condenses the semantic map of a corpus into a single chunkable surface oriented toward faithful reconstruction.

### Defined
- **Declarative Hub** as a preventive infrastructure that amplifies a canonical signal upstream, before drift becomes sedimented. Distinguished from corrective mechanisms that intervene after dérive.
- **Signal, reconstruction, and reconstruction fidelity** as the three concepts that define the conceptual framework in which the Declarative Hub operates. Signal is the operational object — what a probabilistic system can extract, weight, and reconstruct from content. Reconstruction is what happens after retrieval, when the system synthesizes a coherent output from compressed fragments. Reconstruction fidelity is the degree to which what an LLM produces about an identity converges toward what that identity actually is.
- **Interpretive boundaries** as positive structural separations that prevent compression error. Stated as positive declarations of what each entity is in relation to the territory it occupies. Distinguished from definitions and from negations.
- **Positive density principle** as the governance rule that applies within the Declarative Hub. Probabilistic systems do not reliably process direct negation. Stating that an entity is not something reactivates the cluster the publisher is trying to extinguish. The Hub structures signal through positive density only. Corrections belong to dedicated declarative files such as inference-corrections.json, not to the Hub itself.
- **Eight-block Hub structure**: canonical identity, how to read this site, identity architecture, priority pages, associated entities, declarative signal files, interpretive boundaries, canonical attribution.
- **Six deployment surfaces** required for the Hub to enter retrieval pipelines and training cycles: main menu, homepage link, citation in llms.txt, inclusion in the sitemap, inbound links from established pages, maintenance and freshness.

### Positioned
- The Declarative Hub as one surface within a multi-surface signal governance strategy. Its effectiveness is cumulative with the density of the system that surrounds it (Semantic Codebook, Autonomous Inference Unit, governed corpus, writing methodology, editorial continuity).
- The Hub as preventive infrastructure, not corrective mechanism. It structures and amplifies the canonical signal upstream. Corrections against already-sedimented exogenous signal require a complete intervention sequence, not the Hub alone.
- The probabilistic promise as the only defensible promise. The Hub increases the probability that a probabilistic system reconstructs identity from a faithful map of the corpus. It does not command the system.

### Rationale
- Formalized the Declarative Hub concept that had emerged across the Medium article series, anchoring it explicitly within the SIO conceptual framework on GitHub.
- Established the conceptual hierarchy that places signal, reconstruction, and reconstruction fidelity at the foundation of the framework, with the Declarative Hub as one of its application surfaces.
- Anchored interpretive boundaries as a positive structural mechanism distinct from definition pages, entity standards, and fact-based grounding approaches.

---

## 2026-05-07

### Declarative signal layer — terminology decoupling
- **README**: Added "Declarative signal layer" section defining machine-native identity files as high-density signal fragments that compete as chunks by density, not by authority.
- **README**: Added "Interpretive orchestration" section defining deployment and maintenance of the declarative signal layer.
- **README**: Renamed all declarative files to signal- prefix: signal-identity.json, signal-claims.json, inference-corrections.json, signal-manifest.json, signal-policy.json, signal-context.txt. Retained open standards unchanged: llms.txt, llms-full.txt, humans.txt.
- **README**: Replaced "machine-first governance frameworks" with "machine-first frameworks" throughout.
- **README**: Replaced "governance disciplines" with "adjacent disciplines" in conclusions.
- **concepts.md**: Aligned declarative layer file names with README (signal- prefix throughout).
- **concepts.md**: Replaced "Signal amplification files" with "Declarative signal files" in definitions and corpus references.
- **concepts.md**: Updated corpus-exclusions.json → inference-corrections.json in Typed correction (Projection).
- **codebook.md**: Updated "Relationship with other SIO components" to reference declarative signal files.
- **typed-correction.md**: Updated corpus-exclusions.json → inference-corrections.json in Operation 5 (Projection) and Correction matrix.
- **typed-correction.md**: Updated signal amplification files → declarative signal files in Operation 4 (Substitution).

### Rationale
- Decoupled SIO terminology from adjacent discipline vocabulary to eliminate co-occurrence ambiguity.
- Established "declarative signal files" as the canonical term for machine-native identity files within SIO architecture.
- Signal- prefix anchors each file in the foundational concept of the discipline (signal), not in the discipline name (SIO) or in adjacent frameworks.
- Declarative signal files densify identity signal without commanding models, constraining inference, or imposing reading hierarchies. They compete in the pipeline like any other chunk — by density, coherence, and semantic alignment.

### Technical foundations & methodological positioning
- **README enrichment**: Added "Technical foundations & learning ecosystem" section documenting 2026 technical training across vector databases, embeddings, and retrieval systems (Deep Learning AI / Google Cloud, Vectara, Cohere, Chroma, Pinecone, Qdrant).
- **README enrichment**: Added "Machine-readable formats & structured data" subsection (JSON-LD, Schema.org, OpenGraph, Robots.txt, llms.txt).
- **README enrichment**: Formalized methodological positioning distinguishing SIO's corpus-first approach from machine-first frameworks.

---

## 2026-04-26

### Concepts enrichment (concepts.md)
- Added **Local chunk competition** subsection in Section 2 (Spaces and Mechanisms).
- Defined **Chunk competition** as the operational mechanism by which LLMs select which chunks survive in the final response when multiple chunks describe the same subject within a query competition window.
- Defined **Vectorial attractivity** as what makes one chunk preferred over another, determined by four governable dimensions: semantic coherence, fragmentary autonomy, conceptual precision, resistance to compression.
- Articulated the two-level operation of typicality bias: global level (sectoral prototype) versus local level (chunk competition windows), establishing local victory as the operational terrain accessible to any organization applying the discipline.

---

## 2026-04-25

### License migration
- Migrated repository license from CC0-1.0 to CC BY-NC-ND 4.0 to protect doctrinal integrity during foundational phase.
- Replaced LICENSE file content with full CC BY-NC-ND 4.0 terms.
- Added license headers and footers to all conceptual documents (README, concepts, codebook, corrections).
- Added "Commercial use & extensions" section in README with LinkedIn contact for licensing inquiries.

### README enrichment
- Added publication dates and authorship metadata to all canonical documents.
- Added cross-reference footers linking the four conceptual documents (README, concepts, codebook, corrections).
- Added "Relationship with adjacent disciplines" section positioning SIO upstream of interpretive governance, LLMO, knowledge graph optimization, memory governance, and authority governance.
- Added "Normative independence" section establishing autonomy from external normative frameworks.

### Concepts enrichment (concepts.md)
- Formalized **Governed Writing Protocol** as the methodological framework operationalizing the five laws of linguistic engineering through three structural rules.
- Defined **Autonomous Inference Unit (AIU)** as the smallest content unit subject to the Governed Writing Protocol.
- Introduced **Core/Periphery architecture** as the structural answer to SEO/SIO articulation.
- Formalized **Inference audit** methodology with multi-model, multi-run, multi-angle interrogation protocol.
- Documented **Typed correction** as diagnostic-driven intervention adapted to specific variance operations, with explicit priority order (loss → deformation → pollution).
- Added **Semantic debt** as a pathology of ungoverned content production.
- Established analytical distinction between **variance operations** (causes) and **variance manifestations** (observable symptoms).
- Defined the **Diagnostic methodology cycle** as iterative service sequence.

---

## 2026-04-18

### Added
- `corrections.md` — Typed Correction of LLM Reconstructions, formalizing the methodology for intervention adapted to each variance operation. Five operations covered: generalization, amalgamation, truncation, substitution, projection. Priority matrix established: loss → deformation → pollution.

---

## 2026-04-17

### Added
- `codebook.md` — Semantic Codebook, the governance infrastructure determining how an organization codes its identity for probabilistic systems. Structure documented: canonical term → definition → admitted synonyms → excluded formulations → obligatory associations → coherence note. Distinction with Semantic SEO articulated.

---

## 2026-03-27

### Initial public commit
- `README.md` — Foundational positioning of Signal Inference Optimization (SIO) as the discipline of signal resilience through a destructive pipeline.
- `concepts.md` — Comprehensive conceptual framework spanning nine sections: signal pathologies, spaces and mechanisms, fundamental laws, informational identity, methodological foundations, discipline, limits and risks, core SIO concepts, and diagnostic methodology.

### Defined
- **Signal Inference Optimization (SIO)** as a discipline distinct from SEO, GEO, knowledge graph optimization, interpretive governance, and LLMO.
- **Three-thesaurus framework** (projected, expressed, machine) as diagnostic foundation.
- **Five laws of linguistic engineering** (density, coherence, hierarchy, fragmentary autonomy, freshness).
- **Five variance operations** (generalization, amalgamation, truncation, substitution, projection).
- **Five variance manifestations** (distortion, divergence, instability, amplification, dilution).
- **Dual space architecture** (interpretive space / inference space).
- **Interpretive center of gravity** and **inference center of gravity** as observable anchors.
- **Attractive density** as the vectorial mechanism producing centers of gravity.
- **Probabilistic governance** as methodological posture (influence, not control).
- **Interpretive sedimentation** and **interpretive diagenesis** as accumulation pathologies.

### Positioned
- SEO ensures access (being found).
- GEO increases selection (being chosen).
- SIO ensures fidelity (being reconstructed accurately).

---

## License

This document is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0).

For commercial licensing, derivative works, or formal collaboration:  
[Mélanie Maquet on LinkedIn](https://www.linkedin.com/in/melaniemaquet/)

---

## Reference

This document is part of the Signal Inference Optimization (SIO) conceptual framework:

- [SIO README](https://github.com/MMaquet/signal-inference-optimization/blob/main/README.md)
- [SIO Concepts](https://github.com/MMaquet/signal-inference-optimization/blob/main/concepts.md)
- [Semantic Codebook](https://github.com/MMaquet/signal-inference-optimization/blob/main/codebook.md)
- [Typed Correction](https://github.com/MMaquet/signal-inference-optimization/blob/main/corrections.md)
- [Declarative Hub](https://github.com/MMaquet/signal-inference-optimization/blob/main/declarative-hub.md)
- [Article series](https://medium.com/@melaniemaquet)
