> **License:** This work is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
> Attribution required. No commercial use. No derivatives.
> See [LICENSE](./LICENSE) file.

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

**First public commit:** April 18, 2026  
**Last updated:** April 25, 2026  
**Author:** Mélanie Maquet

---

# Typed Correction of LLM Reconstructions

Probabilistic systems do not produce random errors.  
They deform signals through identifiable operations.

Each operation has a structural cause, an observable effect, and a specific correction.

Generic correction — publishing more content — fails because it ignores this specificity.  
Typed correction identifies the dominant operation and applies the corresponding structural intervention.

---

## Diagnostic framework

### Five diagnostic questions

Each question identifies a specific variance operation:

- **Does the reconstruction describe my category rather than my expertise?** → **Generalization**
- **Does the reconstruction merge me with my competitors or my sector?** → **Amalgamation**
- **Is the reconstruction partially correct but incomplete?** → **Truncation**
- **Is my proprietary term replaced by a generic equivalent?** → **Substitution**
- **Does the reconstruction contain attributes I never published?** → **Projection**

### Multicausality

In practice, variance operations are often combined. A reconstruction can be simultaneously generalized and truncated. Typed correction identifies the dominant operation — the one whose correction will produce the most structural effect — and prioritizes accordingly.

### Priority order: loss → deformation → pollution

When multiple operations are active simultaneously, triage follows a structural principle:

**Priority 1 — Identity loss: amalgamation and substitution.**  
Differentiation has disappeared. The organization is interchangeable with competitors or its proprietary term has been neutralized. Without distinct identity in the inference space, no other correction has effect. Treat first.

**Priority 2 — Identity deformation: generalization.**  
The organization exists but in generic version. The signal is present but distorted. Treat second.

**Priority 3 — Incomplete signal: truncation.**  
Positioning is partially correct but amputated. Repairable through reinforcement of obligatory associations between concept components. Treat third.

**Priority 4 — Polluted signal: projection.**  
The model added unfounded attributes. This is noise, not loss. Correction through density and machine-readable declaration is the slowest to produce effects. Treat last.

---

## Operation 1 — Generalization

**Mechanism:** The model broadens the organization's scope beyond actual identity. A pointed expertise is reconstructed in its broadest categorical version.

**Detection in inference audit:** Direct queries produce responses describing the sectoral category rather than the distinctive expertise. Generic sector terms dominate. Proprietary terms appear in secondary position or disappear.

**Dominant cause:** The central concept is not sufficiently dense in the corpus — insufficient repetition, insufficient stable co-occurrences. Or peripheral concepts are denser than the central concept.

**Typed correction:**
- Densify the central concept — increase canonical term frequency in endogenous corpus, reinforce co-occurrences with obligatory associations, produce pillar content where the central concept dominates
- Reduce relative weight of peripheral signals — identify content where generic terms dominate and rewrite to restore hierarchy. Rebalancing is sometimes a question of pruning, not additional production

---

## Operation 2 — Amalgamation

**Mechanism:** The model merges the organization with competitors or with the entire sectoral category. Identity boundaries dissolve. The organization becomes an interchangeable representative of its category.

**Detection in inference audit:** Comparative queries produce responses that find no clear distinction. Direct queries produce descriptions applicable to any sector actor.

**Dominant cause:** The organization's corpus uses the same vocabulary as its competitors. Same terms, same associations, same formulations. The model finds no distinctive signal sufficient to separate entities.

**Typed correction:**
- Reinforce proprietary concepts — identify or create terms no one else uses. The named methodology, the proprietary conceptual framework, the expressions that belong only to this organization. Repeat with intention and coherence across the entire corpus
- Exclude shared terms from the conceptual core — terms all competitors use should not occupy the center of the signal. They may appear in context. They must not be in the conceptual nucleus. The Codebook formalizes this exclusion

---

## Operation 3 — Truncation

**Mechanism:** The model retains only part of the positioning. The complete expertise is amputated. What remains is correct but incomplete, and incompleteness changes meaning.

**Detection in inference audit:** Distinctive attributes disappear from reconstructions. Pointed queries do not cite the organization. Generic queries cite it without distinction.

**Dominant cause:** The concept is composite — multiple words that must stay together to carry complete meaning. During probabilistic compression, the model tends to retain the word with the most statistical mass alone and eliminate qualifying terms. The concept's components are not sufficiently linked in the corpus to resist separation.

**Typed correction:**
- Reinforce obligatory associations between concept components — every time the root term appears in the corpus, the qualifying term must be nearby. The objective is to create a co-occurrence so stable that the model cannot separate the components. In vector space, both terms must occupy positions close enough to form a single cluster
- This is not mechanical repetition. It is co-occurrence engineering — same terms, in varied but always joint contexts, so their association becomes a statistical regularity the model retains

---

## Operation 4 — Substitution

**Mechanism:** The model replaces a proprietary concept with its generic sectoral equivalent. The term the organization built, defined, and publicly established disappears in favor of standard vocabulary.

**Detection in inference audit:** The proprietary term does not appear in reconstructions. It is systematically replaced by the generic equivalent. Queries using the proprietary term may produce responses that do not cite the organization that created it.

**Dominant cause:** The generic term is massively denser in the global interpretive space — thousands of sources use it. The proprietary term exists in a limited endogenous corpus. Statistical mass asymmetry favors the generic during reconstruction.

**Typed correction:**
- Exclude the generic term from the Codebook — it must not appear as a central term in the corpus. It may exist in context, as explicit contrast, never as equivalent
- Densify the proprietary term — it must appear in every pillar content, governance files, structured metadata, satellite content. Frequency must be sufficient to create an autonomous cluster
- Create explicit contrastive associations — produce content that explicitly opposes the proprietary term to the generic: "X is not Y. It intervenes upstream, on the structure itself." This creates a contrastive association in the inference space — the model learns the two terms are not synonymous

---

## Operation 5 — Projection

**Mechanism:** The model attributes properties the organization does not have, because these properties are statistically typical of its category. The organization published nothing on the subject. The model inferred it.

**Detection in inference audit:** Attributes appear in reconstructions with no identifiable source in the endogenous corpus. Pointed queries receive affirmative responses based on no real signal.

**Dominant cause:** The corpus does not explicitly state what the organization does NOT do. The model fills silence zones with what is statistically probable for the category. Silence is not neutral in a probabilistic system — it is an invitation to project.

**Typed correction:**
- Massively densify the real signal — if the corpus is saturated with the actual expertise and strong, specific obligatory associations, less vector space remains available for generic projections. Real signal density mechanically reduces the space available for unfounded inference
- Declare in common-misinterpretations.json — this is exactly what this governance file serves in interpretive orchestration. Explicitly declare in machine-readable format what the organization is NOT
- Do NOT contradict in editorial content — writing "We do NOT do X" creates a co-occurrence between the organization and X. The model may ignore the negation and retain the association. Correction passes through real signal density and machine-readable declaration, not editorial negation

---

## Correction matrix

| Operation | Diagnostic question | Correction |
|---|---|---|
| Generalization | Category instead of expertise? | Densify central concept + reduce peripheral weight |
| Amalgamation | Merged with competitors? | Reinforce proprietary concepts + exclude shared terms |
| Truncation | Correct but incomplete? | Reinforce obligatory associations between components |
| Substitution | Proprietary term replaced? | Exclude generic + densify proprietary + contrastive associations |
| Projection | Unpublished attributes added? | Densify real signal + declare in common-misinterpretations.json |

---

## Priority matrix

| Priority | Type | Operations | Principle |
|---|---|---|---|
| 1 | Identity loss | Amalgamation, Substitution | Without distinct identity, nothing else matters |
| 2 | Identity deformation | Generalization | Signal present but distorted |
| 3 | Incomplete signal | Truncation | Signal present but amputated |
| 4 | Polluted signal | Projection | Noise added, not signal lost |

Structural principle: **loss → deformation → pollution.**  
Restore what disappeared. Correct what is distorted. Clean what was added.

---

## Limits

Typed correction does not guarantee reconstruction correction. The box remains opaque. The model remains probabilistic. Correction is an intervention on inputs whose effect on outputs is observable but not guaranteed.

Typed correction does not produce immediate effects. Latency between corrective signal injection and integration in reconstructions varies by model, update cycle, and retrieval mechanism. Latency is structural, not accidental.

Some deformations resist endogenous correction because their cause is primarily exogenous — a competing signal massively denser in the global interpretive space. In these cases, typed correction reduces the deformation without eliminating it. Recognizing this limit is part of the discipline.

Typed correction requires prior diagnosis — a systematic inference audit that identifies not only that reconstruction is deformed, but which type of deformation is active. Without diagnosis, correction remains generic. And generic correction in a probabilistic system is random correction.

**Typed correction is applied probabilistic governance. Not control. A structured, measurable, repeatable intervention — in a system no one controls.**

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
- [SIO Concepts](https://github.com/MMaquet/signal-inference-optimization/blob/main/concepts.md)
- [Semantic Codebook](https://github.com/MMaquet/signal-inference-optimization/blob/main/codebook.md)
- [Article series](https://medium.com/@melaniemaquet)

**First public commit:** April 18, 2026  
**Last updated:** April 25, 2026  
**Author:** Mélanie Maquet — SEMANTIKIA
