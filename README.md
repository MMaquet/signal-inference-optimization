# Signal Inference Optimization (SIO) 

> **License:** This work is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
> Attribution required. No commercial use. No derivatives.
> See [LICENSE](./LICENSE) file.

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

LLMs do not retrieve your content.  
They reconstruct it.

What they reconstruct becomes your identity.

---

**First public commit:** March 27, 2026  
**Last updated:** July 4, 2026  
**Author:** Mélanie Maquet — SEMANTIKIA

---

## Definition

Signal Inference Optimization (SIO) is the discipline of structuring 
the signal made available to probabilistic systems in order to reduce 
inference drift and orient LLM reconstructions toward a version that 
remains faithful to the intended meaning.

SIO does not optimize inference.  
It optimizes the signal that enters the inference process.

SIO does not control reconstruction.  
It structures the conditions that make faithful reconstruction more likely.

The name reads: optimization of the signal **for** inference —  
not optimization **of** inference itself.

**SIO is the discipline of signal resilience through a destructive pipeline.**

---

## Repository map

- [Conceptual framework](./concepts.md) — core concepts, mechanisms, laws, diagnostic methodology
- [Semantic Codebook](./codebook.md) — terminological governance infrastructure
- [Typed corrections](./corrections.md) — variance operations and correction pathways
- [Declarative Hub](./declarative-hub.md) — visible compression surface for canonical signal
- [Technical foundations](./technical-foundations.md) — technical systems SIO is built to account for
- [Changelog](./changelog.md) — doctrine evolution

---

## Core shift

In traditional systems, meaning is retrieved.  
In probabilistic systems, meaning is reconstructed.

You are no longer indexed.  
You are inferred.

---

## Positioning

- **SEO** — ensures access: being found  
- **GEO** — increases selection: being chosen  
- **SIO** — ensures fidelity: being reconstructed accurately  

SEO makes you visible.  
GEO makes you selectable.  
SIO determines what you become.

---

## The problem

Probabilistic systems compress and reconstruct information.

During this process:

- signals are fragmented  
- context is reduced  
- meaning is approximated  
- responses may be cached and re-served by application layers  

Unstructured signals drift.  
Drift produces distortion.  
Distortion becomes representation.

Without SIO, you are not represented.  
You are approximated.

---

## Dual space architecture

SIO operates across two distinct spaces:

- **Interpretive space** — the global informational environment  
  where signals circulate (all corpora, all sources, the full web).  
  This is the signal source. This is where you act.

- **Inference space** — the internal vectorial/probabilistic space  
  of the LLM where embeddings distribute and reconstruction occurs.  
  This is signal processing. This is what you influence.

You govern the interpretive space.  
The model operates in the inference space.  
Inference drift is the gap between the two.

---

## Inference pipeline

All signals pass through transformation pipelines.  
The exact architecture varies by system, but common patterns emerge.

### Single-hop (typical pattern)

Query analysis → Query expansion → Web search → Page selection →  
Extraction → Semantic chunking → Embedding → Hybrid retrieval →  
Reranking → Context construction → Generation → Delivery

### Multi-hop (complex queries)

Complex queries may trigger parallel pipelines:

Query fan-out → Parallel single-hop pipelines per sub-query →  
Local synthesis → Synthesis fusion → Global context → Final generation

At each stage, information is transformed.  
At multiple critical points, signal can degrade or disappear.

After generation, the response may also pass through a delivery layer:  
semantic cache, application orchestration, response filters, or reuse policies.  
This layer can preserve, distort, or freeze a reconstruction independently  
of the current corpus.

SIO structures the signal to preserve semantic coherence  
across pipeline variations.

See detailed analysis:  
https://github.com/MMaquet/signal-inference-optimization/blob/main/concepts.md

---

## Inference drift

Inference drift is the deviation between intended meaning and 
reconstructed output — the gap between what enters the interpretive 
space and what emerges from the inference space.

Signal degradation accumulates across the transformation pipeline.  
At multiple critical points, signals can degrade or disappear entirely.

SIO structures signals to resist this degradation and preserve 
semantic coherence through the reconstruction process.

See detailed analysis:  
https://github.com/MMaquet/signal-inference-optimization/blob/main/concepts.md

---

## Signal survival

Structuring the signal is necessary.  
But the real standard is survival.

A signal must survive the inference pipeline intact —  
chunking, embedding, retrieval, reranking, generation —  
and emerge in reconstruction faithful to its original meaning.

If the signal does not survive,  
its meaning does not exist in the system.

SIO is the discipline of making signal survival intentional.

---

## Semantic caching and application-layer fixation

SIO primarily governs the signal made available to probabilistic systems.  
But users do not always receive a fresh native model reconstruction.

In deployed AI applications, a generated response may be stored in a  
semantic cache and reused for semantically similar queries. This creates  
a distinct fidelity risk: one probabilistic output can be frozen and  
served repeatedly as if it were the canonical response.

This mechanism is called **stochastic fixation**.

Stochastic fixation differs from interpretive sedimentation:

- **Interpretive sedimentation** consolidates slowly through corpus ingestion,  
  republication, and model update cycles.
- **Stochastic fixation** operates at delivery time, when an application layer  
  captures one model output and re-serves it through cache or orchestration.

This distinction introduces two diagnostic objects:

- **Native machine thesaurus** — what the model reconstructs through direct interrogation.
- **Delivered machine thesaurus** — what a deployed application actually serves to users.

A corpus can be current, coherent, and well-governed while an application  
continues serving an older cached reconstruction. In that case, the problem  
is not only inference drift. It is delivery drift.

The corpus governs the conditions of reconstruction.  
It does not directly govern the cache.

---

## Declarative signal layer

The editorial corpus produces signal through statistical accumulation.  
The declarative signal layer produces signal through explicit declaration  
in machine-native formats.

These are not instructions to the model.  
These are not constraints on inference.  
These are high-density signal fragments in formats that machines parse natively.

A 200-word signal-identity.json produces a denser chunk  
than a 2000-word blog post. The signal-per-token ratio is higher.

### Declarative signal files

| File | Function |
|---|---|
| **llms.txt** | Signal entry point — content index in LLM-readable format (open standard, Jeremy Howard) |
| **llms-full.txt** | Extended signal documentation — complete organizational description optimized for LLM ingestion (open standard, Jeremy Howard) |
| **signal-identity.json** | Identity declaration — who the organization is, in structured format |
| **signal-claims.json** | Canonical assertions — what the organization affirms as its positioning |
| **inference-corrections.json** | Reconstruction corrections — identified inference errors and their factual corrections |
| **signal-manifest.json** | Structured metadata — entity type, mission, scope, version |
| **signal-policy.json** | Usage policy — conditions under which content may be used by AI systems |
| **signal-context.txt** | Representation context — how the organization should be represented |
| **humans.txt** | Human attribution — people behind the organization (open standard since 2009) |

### What declarative signal files do

Declarative signal files densify the identity signal in machine-native format.  
They do not command the model. They do not constrain inference.  
They compete as chunks — and win by density when properly structured.

A declarative signal layer without a governed corpus  
declares an identity the corpus does not carry.

A governed corpus without a declarative signal layer  
is under-exploited — the densest identity fragments are missing.

Both are necessary. Neither is sufficient alone.

### What declarative signal files do not do

They do not control LLM reconstructions.  
They do not guarantee indexation or integration.  
They do not override corpus signals by authority.  
They compete in the pipeline like any other chunk —  
by density, coherence, and semantic alignment.

### Relationship with the Semantic Codebook

Declarative signal files must use the canonical terminology  
of the Semantic Codebook. The same terms, the same associations,  
the same exclusions. Coherence between the editorial corpus  
and the declarative layer is non-negotiable.

---

## Interpretive orchestration

Interpretive orchestration is the deployment and maintenance  
of the declarative signal layer as an integrated component  
of the SIO architecture.

Interpretive orchestration includes:

- Structuring declarative signal files with Codebook-aligned terminology  
- Deploying files at stable, predictable URLs  
- Maintaining coherence between the editorial corpus and the declarative layer  
- Versioning and dating all declarative files  
- Updating when the Codebook evolves  

Interpretive orchestration is the infrastructure component of SIO.  
It does not replace corpus density. It complements it  
by providing a stable, machine-native reference layer.

---

## Centers of gravity

SIO produces two observable anchors:

- **Interpretive center of gravity** — the dominant cluster  
  in the interpretive space. The source signal sufficiently dense  
  and coherent to orient reconstructions. This is what you build.

- **Inference center of gravity** — the convergence point  
  in the inference space toward which embeddings converge.  
  This is what you measure.

**Attractive density** is the mechanism that produces both.

---

## Informational identity

In probabilistic systems, identity is not stored.  
It is reconstructed.

What emerges from inference becomes your informational identity.

This identity is:

- probabilistic  
- context-dependent  
- shaped by available signals  

SIO stabilizes this identity by structuring  
how signals enter the system.

---

## What SIO is not

- Not semantic SEO  
- Not GEO  
- Not knowledge graph optimization  
- Not interpretive governance  
- Not LLMO  

SIO operates upstream.  
It structures what enters the system  
before interpretation, selection, or validation occur.

---

## Relationship with adjacent disciplines

SIO occupies the upstream layer of the inference pipeline. It complements,  
but does not replace, downstream disciplines that operate after signal entry:

- **Interpretive governance** — defines conditions of reading and meaning production  
- **LLMO** — optimizes outputs after reconstruction  
- **Knowledge graph optimization** — structures verifiable entities and attributes  
- **Memory governance** — oversees stateful AI memory systems  
- **Authority governance** — constrains executable AI authority  

These disciplines structure what happens to a signal after it enters the system.  
SIO structures what enters the system in the first place.

A complete approach combines upstream signal structuring (SIO)  
and downstream interpretation conditions (adjacent disciplines).  
Without SIO, downstream disciplines operate on signal that has already drifted.

---

## Technical foundations

SIO is not a technical implementation framework.  
It is a corpus-first discipline built with direct awareness of the technical  
systems that transform, compress, retrieve, reconstruct, cache, and deliver signals.

The technical foundations of SIO are documented separately:

[technical-foundations.md](./technical-foundations.md)

---

## Normative independence

SIO is defined and developed by its author.  
It operates under no external normative authority.

This framework evolves through:

- documented research  
- field practice  
- published case studies  

It is not subject to third-party arbitration  
or distributed authority allocation by external entities.

---

## Conceptual framework

SIO is grounded in a structured conceptual system.

This system defines:

- pathologies of signal degradation  
- mechanisms of probabilistic reconstruction  
- principles of informational identity  
- methods for semantic structuring  
- diagnostic methodology for measuring signal integrity  
- application-layer risks such as semantic caching and stochastic fixation  

See full framework:  
https://github.com/MMaquet/signal-inference-optimization/blob/main/concepts.md

---

## Operational application

SIO is the conceptual framework.  
SEMANTIKIA is the operational application of SIO for organizations.

The conceptual framework is public.  
The operational application is commercial.

This distinction is explicit and locked.

For diagnostics, Semantic Codebooks, inference audits, and corrections:  
[semantikia.com](https://semantikia.com)

---

## Status

This repository establishes the conceptual foundation of SIO.

It will evolve toward:

- inference audit methodologies  
- signal integrity diagnostics  
- operational structuring frameworks  

---

## Author

Mélanie Maquet — originator of Signal Inference Optimization,  
founder of SEMANTIKIA.

[melaniemaquet.com/identite-canonique](https://www.melaniemaquet.com/identite-canonique)  
[sio.melaniemaquet.com](https://sio.melaniemaquet.com)  
[linkedin.com/in/melaniemaquet](https://www.linkedin.com/in/melaniemaquet/)

First public commit: March 27, 2026  
Last updated: July 4, 2026

---

## Writing & research

The SIO doctrinal corpus is accessible through:

https://sio.melaniemaquet.com

The GitHub repository defines the conceptual structure.  
The doctrinal corpus develops reasoning, applications, and implications.

---

## License

This work is licensed under the Creative Commons 
Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0).

You may share this work with attribution.  
You may not use it commercially.  
You may not modify or redistribute modified versions.

Full license text: https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode  
See [LICENSE](./LICENSE) file in this repository.

---

## Commercial use & extensions

This work is currently licensed under CC BY-NC-ND 4.0 — no commercial use, 
no derivatives — to protect the integrity of the discipline during its 
foundational phase.

For commercial licensing, derivative works, formal collaboration, 
or research partnership inquiries, please contact:

**Mélanie Maquet** — [LinkedIn](https://www.linkedin.com/in/melaniemaquet/)

The license may evolve toward broader openness as the discipline 
matures and is validated through field practice. Until then, integrity 
of the foundational vocabulary takes priority over derivative circulation.

---

## Closing

In probabilistic systems:

Visibility is not identity.  
Selection is not control.

What survives reconstruction defines what you are.

SIO is the discipline of making that survival intentional.
