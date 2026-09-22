> **License:** This work is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
> Attribution required. No commercial use. No derivatives.
> See [LICENSE](./LICENSE) file.

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

**Last updated:** September 22, 2026  
**Author:** Mélanie Maquet — SEMANTIKIA

---

# Changelog

All notable changes to the Signal Inference Optimization (SIO) conceptual framework are documented in this file.

This framework follows a deliberate publication cadence — foundational concepts established first, technical operationalization deployed progressively, field validation conducted before public claims.

---

## 2026-09-22

### Version 1.2 — doctrinal architecture, lexical governance, and claim scoping

Applies to `README.md`, `concepts.md`, `codebook.md`, `corrections.md`, and `declarative-hub.md`. All five files carry version 1.2 and the same date.

### Added
- **The three pillars of SIO** — inferential audit, canonical reference formalization, inferential governance. Stated in README, concepts.md (section 8) and codebook.md. Former sections 8 and 9 of concepts.md renumbered to 9 and 10.
- **Lexical family rule**, governing four families across the repository.
- **Declarative Hub** defined in concepts.md and codebook.md as a surface within declarative orchestration, having previously existed only as its own file.
- **Governed translation** of *canonical reference* and *référence déclarée*, inscribed in codebook.md.
- **Declarative governance and embedded governance** as the two vehicles of inferential governance.
- **The five variance manifestations** defined individually in codebook.md alongside the five variance operations.
- **Qualification against the canonical reference** distinguished from diagnostic localization through the two gaps: canonical reference to machine thesaurus qualifies fidelity; projected to expressed and expressed to machine localize where the deviation originates.
- License block, version, date, and author header on `declarative-hub.md`, which had none. Version number on `corrections.md`, which had none.

### Defined
- **Lexical family rule** — where a third party occupies an adjacent territory under a given lexical family, that family is admitted for describing phenomena and excluded for naming the entity's own practices and instruments. Applied to four families: *interpretive* describes the space and what occurs within it; *inference* names mechanisms and spaces; *inferential* names the practices; *declarative* names the machine-format layer.
- **Declarative orchestration** — the deployment, coordination, versioning, and maintenance of the declarative surfaces. Replaces *interpretive orchestration*.
- **Declarative Hub** — a public, indexable HTML surface deployed within declarative orchestration. Three levels remain distinct: the Hub is the surface, declarative orchestration is the infrastructure that deploys it, declarative governance is the normative content it carries.
- **Inferential governance** — replaces *probabilistic governance* and absorbs its epistemic caveat: correlation between signal intervention and reconstruction change is observable; causality is not provable.
- **Boundaries of interpretation** — replaces *interpretive boundaries* in `declarative-hub.md`.

### Changed
- *Interpretive orchestration* becomes *declarative orchestration*, in README, concepts.md and codebook.md.
- *Inference audit* becomes *inferential audit* for the practice. *Inference drift*, *inference pipeline*, *inference space* and *inference center of gravity* are retained: they name mechanisms and spaces.
- *Admitted synonyms* becomes *admitted variants*. The absolute non-synonymization rule for the proprietary conceptual core is replaced by controlled variants: acronyms, governed translations, grammatical variations, and formally admitted short forms.
- The Semantic Codebook entry structure gains *attributions and relationships* and *limits*, and is aligned across concepts.md and codebook.md.
- The five variance manifestations are named in their canonical bare form — distortion, divergence, instability, amplification, dilution — replacing two competing forms within concepts.md.
- The priority order reads *loss → distortion → pollution* in both concepts.md and corrections.md, replacing *deformation* in corrections.md.
- In the README terminology table, the French form of *canonical reference* becomes *référence déclarée*. *Référentiel canonique* is withdrawn.
- **Declarative file inventory unified** under two prefixes: `sio-` designates what the entity declares about itself, `corpus-` designates what its corpus canonically contains or excludes. This reverses the decision of 2026-05-07, which adopted the `signal-` prefix in order to anchor the files in the foundational concept rather than in the discipline name. The reversal is deliberate: README and concepts.md carried two divergent inventories with no overlap on the JSON file names, and a single inventory takes precedence over the earlier rationale. `inference-corrections.json` becomes `sio-corrections.json`. `sio-glossary.json`, `corpus-canon.json` and `corpus-exclusions.json` enter the README inventory with their functions.
- *Signal amplification files* becomes *declarative signal files* in concepts.md. The change was recorded on 2026-05-07 but not applied.
- *Organization* becomes *entity* where it designates the subject of analysis, consistent with the definition of **Entity** in concepts.md.
- In `corrections.md`, *dominant cause* becomes *probable cause* at all five operations.

### Scoped
- **The pipelines** are stated as analytical patterns describing recurrent transformation stages, not as a universal architecture. Query decomposition is presented as one possible retrieval-augmented design.
- **The five signal disappearance points** become five recurrent signal-loss points, stated as conditional.
- **Chunk competition and vectorial attractivity** are restated as properties of the retrieval and reranking stages rather than of model selection. *Lexical alignment* added as a governable dimension.
- **The context window** is restated in tokens of assembled textual context. The previous formulation referred to embeddings, which do not occupy the context window.
- **The law of density** places its cluster in the interpretive space, not in the inference space, consistent with the dual space architecture.
- **The inference center of gravity** is the recurrent representational pattern toward which observed reconstructions tend to converge. It is inferred from repeated observation of outputs, not from inspection of the model's internal state.
- **Attractive density** receives a single canonical definition, replacing two competing entries in concepts.md, and is inferred from observable changes in reconstruction patterns rather than from internal vectorial mechanisms.
- **Semantic mass** contributes to signal availability rather than determining survival.
- **Acknowledgment of presence** attests presence in the delivered output. It no longer claims that citation proves the signal was seen.
- **Signal survival** is the survival of declared meanings, relationships, attributions, and limits, not of literal text.
- **Declarative signal files** no longer claim to win retrieval by density. When retrieved, they enter the same candidate set as any other passage.
- **The Declarative Hub** states what its publication does and does not establish. Training crawlers and real-time retrieval crawlers are distinguished: availability to one does not imply mobilization by the other. A sitemap declares a page to indexing bots; it does not force discovery, crawling, or indexing.
- **Reconstruction fidelity** in `declarative-hub.md` is conformity to the declared canonical reference, not to what an identity actually is.
- **The status of llms.txt, llms-full.txt and humans.txt** is corrected: public proposals and initiatives, not adopted standards.

### Resolved
- **The contradiction between Substitution and Projection on editorial negation.** Substitution prescribes contrastive association — *X is not Y*. Projection forbids editorial negation. The scope of the difference is now stated: under Substitution the generic term is already massively co-occurrent with the entity, so the intervention qualifies an association that already exists; under Projection the attribute is not yet associated, so naming it in order to deny it creates the co-occurrence from nothing.

### Removed
- **Editorial negation of a third-party proprietary term** from the README. Declared exclusions belong in the declarative layer, in `corpus-exclusions.json`, not in repository prose. The adjacent discipline is now designated by a generic descriptor.

### Fixed
- Broken reference to `semantic-codebook.md` in `declarative-hub.md`. The file is `codebook.md`.
- Incomplete cross-reference blocks in `concepts.md`, `corrections.md` and `declarative-hub.md`. Each file now references the other four and `technical-foundations.md`.
- Author line in `declarative-hub.md`, which described the author through a role the Semantic Codebook excludes.
- Author attribution harmonized to *Mélanie Maquet — SEMANTIKIA* across all files.

### Rationale
- A third-party francophone actor occupies the *interpretive* family on an adjacent territory. The lexical family rule resolves what a blanket exclusion could not: *interpretive space* is the spine of the dual architecture and cannot be withdrawn, while *interpretive orchestration* and *interpretive boundaries* named instruments of the discipline and had to move. Description stays; nomination moves.
- The three pillars separate what SIO does from what it describes. Without that separation, the operations of the discipline and the mechanisms it observes were read as one register.
- Claim scoping across the repository responds to a single standard: an assertion about internal model behaviour that cannot be observed from outputs is not defensible before a technical reader. Vector positions, embedding cancellation, training-cycle entry and cache state are not observable from the corpus side. What can be measured is measured; what cannot be measured is named.
- The unified file inventory takes precedence over the 2026-05-07 prefix rationale because two divergent inventories in the same repository produce two incompatible client implementations, which is a heavier defect than the loss of the concept-anchored prefix.

---

## 2026-07-04

### README optimization — repository navigation and delivery-layer risk
- **README**: Added "Repository map" section linking the main doctrinal files: concepts.md, codebook.md, corrections.md, declarative-hub.md, technical-foundations.md, and changelog.md.
- **README**: Added application-layer delivery to the inference pipeline by extending the single-hop sequence from Generation to Generation → Delivery.
- **README**: Added response caching as an explicit degradation point in "The problem".
- **README**: Added "Semantic caching and application-layer fixation" section defining the delivery-layer risk created when AI applications store and re-serve generated responses.
- **README**: Replaced the long "Technical foundations & learning ecosystem" section with a concise "Technical foundations" section linking to the dedicated technical-foundations.md page.
- **README**: Updated "Conceptual framework" scope to include application-layer risks such as semantic caching and stochastic fixation.
- **README**: Updated last-updated metadata to 2026-07-04.

### Added
- `technical-foundations.md` — Technical Foundations of Signal Inference Optimization. Defines the technical claim of SIO and documents the systems SIO accounts for: retrieval, embeddings, vector search, RAG and grounding pipelines, machine-readable formats, declarative signal infrastructure, semantic caching, and delivery layers.

### Defined
- **Technical claim of SIO**: SIO is not a technical implementation framework. It is a corpus-first discipline built with direct awareness of the technical systems that transform, compress, retrieve, reconstruct, cache, and deliver signals.
- **Semantic caching and application-layer fixation** as a delivery-layer fidelity risk: a probabilistic output can be stored, associated with semantically similar queries, and re-served as if it were canonical.
- **Stochastic fixation** as the mechanism by which one model output, produced under probabilistic conditions, is frozen by an application layer and redistributed through cache or orchestration.
- **Native machine thesaurus** as what the model reconstructs through direct interrogation.
- **Delivered machine thesaurus** as what a deployed application actually serves to users after caching, orchestration, routing, filtering, or reuse policies.

### Positioned
- Semantic caching as a structural limit adjacent to, but distinct from, interpretive sedimentation. Sedimentation consolidates slowly through corpus ingestion, republication, and model update cycles. Stochastic fixation operates at delivery time, when an application layer captures one model output and re-serves it.
- The delivery layer as a new diagnostic concern for SIO: a corpus can be current, coherent, and well-governed while an application continues serving an older cached reconstruction.
- `technical-foundations.md` as a credibility and boundary-setting document. It clarifies the technical systems SIO is built to account for while explicitly stating what SIO does not claim: it does not control LLM outputs, command models through files, replace technical SEO, replace knowledge graphs, replace RAG engineering, guarantee citation, or guarantee cache invalidation.
- The README as the repository entry point rather than the full conceptual framework. Detailed conceptual material remains in concepts.md; technical grounding now lives in technical-foundations.md.

### Rationale
- Added a repository map to make the GitHub project easier to navigate and to separate entry-point, conceptual, methodological, declarative, corrective, and technical materials.
- Moved technical foundations out of the README to prevent the repository homepage from reading as a training inventory. The new technical-foundations.md page preserves technical credibility while protecting the corpus-first positioning of SIO.
- Integrated semantic caching into the README because the article on stochastic fixation introduces a new structural limit: corpus engineering can influence native reconstruction, but it cannot directly govern cached responses served by application layers.
- Established the native/delivered distinction as necessary for future inference audits. Without this distinction, an application-layer fixation can be misdiagnosed as a corpus failure or native model drift.

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
- [Technical Foundations](https://github.com/MMaquet/signal-inference-optimization/blob/main/technical-foundations.md)
- [Article series](https://medium.com/@melaniemaquet)
