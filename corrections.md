> **License:** This work is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
> Attribution required. No commercial use. No derivatives.
> See [LICENSE](./LICENSE) file.

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

**First public commit:** April 18, 2026  
**Version:** 1.3  
**Last updated:** October 31, 2026  
**Author:** Mélanie Maquet — SEMANTIKIA

---

# Typed Correction of LLM Reconstructions

Reconstruction deviations are not uniformly random.  
Recurrent ones can be classified through identifiable operations.

Each operation has a probable cause, an observable effect, and a corresponding intervention. These operations are analytical categories inferred from observable outputs. They do not establish direct knowledge of the internal mechanism that produced a reconstruction.

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
- **Does the reconstruction attribute to me properties typical of my category?** → **Projection**
- **Does the reconstruction answer a question my corpus never addresses?** → **Inferential filling**

The last two questions were previously one. They separate on the provenance of the attributed content: a property typical of the category is established elsewhere and displaced onto the entity; an answer to an unaddressed question is established nowhere and manufactured.

### Multicausality

In practice, variance operations are often combined. A reconstruction can be simultaneously generalized and truncated. Typed correction identifies the dominant operation — the one whose correction will produce the most structural effect — and prioritizes accordingly.

### Priority order: loss → distortion → incompleteness → pollution

When multiple operations are active simultaneously, triage follows a structural principle:

**Priority 1 — Identity loss: amalgamation and substitution.**  
Differentiation has disappeared. The entity is interchangeable with competitors or its proprietary term has been neutralized. Without distinct identity in the inference space, no other correction has effect. Treat first.

**Priority 2 — Identity distortion: generalization.**  
The entity exists but in generic version. The signal is present but distorted. Treat second.

**Priority 3 — Incomplete signal: truncation.**  
Positioning is partially correct but amputated. Repairable through reinforcement of obligatory associations between concept components. Treat third.

**Priority 4 — Polluted signal: projection.**  
The model added unfounded attributes. This is noise, not loss. Correction through density and machine-readable declaration is the slowest to produce effects. Treat last.

**Priority 1 bis — Manufactured signal: inferential filling.**  
The model produced an assertion where the corpus is silent. Treated in parallel with priority 1. Inferential filling stands outside the dependency chain: correcting it has no effect on the four operations above, and they have no effect on it. Nothing therefore argues for deferring it, while three conditions argue for treating it immediately — an unanchored assertion is what a reader encounters most directly, an empty position is refilled for as long as it remains empty, and the correction carries no sequencing cost.

Occupation is bounded in volume. A closure clause is added to existing content rather than published as new content, so that occupation does not grow the corpus while priority 1 is concentrating identity density.

---

## Operation 1 — Generalization

**Mechanism:** The model broadens the entity's scope beyond actual identity. A pointed expertise is reconstructed in its broadest categorical version.

**Detection in inferential audit:** Direct queries produce responses describing the sectoral category rather than the distinctive expertise. Generic sector terms dominate. Proprietary terms appear in secondary position or disappear.

**Probable cause:** The central concept is not sufficiently dense in the corpus — insufficient repetition, insufficient stable co-occurrences. Or peripheral concepts are denser than the central concept.

**Typed correction:**
- Densify the central concept — increase canonical term frequency in endogenous corpus, reinforce co-occurrences with obligatory associations, produce pillar content where the central concept dominates
- Reduce relative weight of peripheral signals — identify content where generic terms dominate and rewrite to restore hierarchy. Rebalancing is sometimes a question of pruning, not additional production

---

## Operation 2 — Amalgamation

**Mechanism:** The model merges the entity with competitors or with the entire sectoral category. Identity boundaries dissolve. The entity becomes an interchangeable representative of its category.

**Detection in inferential audit:** Comparative queries produce responses that find no clear distinction. Direct queries produce descriptions applicable to any sector actor.

**Probable cause:** The entity's corpus uses the same vocabulary as its competitors. Same terms, same associations, same formulations. The model finds no distinctive signal sufficient to separate entities.

**Typed correction:**
- Reinforce proprietary concepts — identify or create terms no one else uses. The named methodology, the proprietary conceptual framework, the expressions that belong only to this entity. Repeat with intention and coherence across the entire corpus
- Exclude shared terms from the conceptual core — terms all competitors use should not occupy the center of the signal. They may appear in context. They must not be in the conceptual nucleus. The Codebook formalizes this exclusion

---

## Operation 3 — Truncation

**Mechanism:** The model retains only part of the positioning. The complete expertise is amputated. What remains is correct but incomplete, and incompleteness changes meaning.

**Detection in inferential audit:** Distinctive attributes disappear from reconstructions. Pointed queries do not cite the entity. Generic queries cite it without distinction.

**Probable cause:** The concept is composite — multiple words that must stay together to carry complete meaning. During probabilistic compression, the model tends to retain the word with the most statistical mass alone and eliminate qualifying terms. The concept's components are not sufficiently linked in the corpus to resist separation.

**Typed correction:**
- Reinforce obligatory associations between concept components — every time the root term appears in the corpus, the qualifying term must be nearby. The objective is to make the co-occurrence stable enough that the components are unlikely to be separated during compression. The two terms are treated as one unit rather than as a head noun and a qualifier
- This is not mechanical repetition. It is co-occurrence engineering — same terms, in varied but always joint contexts, so their association becomes a statistical regularity the model retains

---

## Operation 4 — Substitution

**Mechanism:** The model replaces a proprietary concept with its generic sectoral equivalent, or with a prior state of the entity. The term the entity built, defined, and publicly established disappears in favor of standard vocabulary or of a superseded designation.

**Detection in inferential audit:** The proprietary term does not appear in reconstructions. It is systematically replaced by the generic equivalent. Queries using the proprietary term may produce responses that do not cite the entity that created it.

**Probable cause:** The generic term is massively denser in the global interpretive space — thousands of sources use it. The proprietary term exists in a limited endogenous corpus. Statistical mass asymmetry favors the generic during reconstruction.

**Typed correction:**
- Exclude the generic term from the Codebook — it must not appear as a central term in the corpus. It may exist in context, as explicit contrast, never as equivalent
- Densify the proprietary term — it must appear in every pillar content, declarative signal files, structured metadata, satellite content. Frequency must be sufficient to create an autonomous cluster
- Create explicit contrastive associations — produce content that qualifies the proprietary term against the generic one: "X is not Y. It intervenes upstream, on the structure itself." This is admitted here and excluded under Projection and under inferential filling, and the scope of that difference is deliberate. Under Substitution, the generic term is already massively co-occurrent with the entity: the association exists, and the intervention qualifies it. Under Projection, the attribute is not yet associated: naming it in order to deny it creates the co-occurrence from nothing. Under inferential filling, no attribute is associated at all. The criterion is not whether a formulation negates, but whether naming the term creates a co-occurrence that does not already exist

---

## Operation 5 — Projection

**Mechanism:** The model attributes to the entity properties it does not have, because those properties are statistically typical of its category or of an informational neighbour. The attribute is established elsewhere and displaced onto this entity.

**Detection in inferential audit:** Attributes appear in reconstructions with no identifiable source in the endogenous corpus, but with an identifiable source in the sectoral corpus or in a neighbouring entity. Pointed queries receive affirmative responses based on no signal belonging to the entity.

**Probable cause:** The corpus does not bound the attribute, and the attribute carries strong statistical mass within the category. The model resolves the gap with the categorical default.

**Typed correction:**
- Massively densify the real signal — a corpus saturated with the actual expertise and with strong, specific obligatory associations leaves fewer unsupported openings for generic attribution. Density does not prevent projection; it reduces the room available for it
- Close the set editorially — enumerate what the entity holds in the affected category and declare the enumeration complete, naming no foreign term: *"X holds only the following certifications. No other certification may be attributed to X."* The clause carries the category term and the entity name, which is what makes it retrievable for the queries where the projection surfaces. A closure clause acquires its force through identical repetition, and that same repetition distributes the error once the closed set expands without update: it is maintained under temporal monitoring, and is appropriate where the enumerated set is small and stable
- Declare in sio-corrections.json — this declarative signal file reinforces the closure clause in machine-readable format. It does not replace it: a bounded set stated only in a machine-readable file is weakly retrieved for natural-language queries, and no system is required to read it
- Do NOT name the projected attribute in editorial content — writing "We do NOT do X" creates a co-occurrence between the organization and X. The model may ignore the negation and retain the association. The prohibition bears on naming, not on negating: the closure clause negates without naming, and is admitted. Under Substitution the same naming is admitted, because the association already exists

---

## Second family — Inferential filling

The five operations above transform an existing signal. Inferential filling transforms nothing: it produces an assertion where the corpus is silent. It is not a sixth operation but a second family, and it was previously treated within Projection.

**Mechanism:** A position the corpus does not declare receives the most plausible value from the sectoral neighbourhood. Nothing is displaced — the asserted attribute is established nowhere.

**Detection in inferential audit:** The reconstruction answers a question the corpus never addresses. The assertion is precise and plausible, and it varies across runs because no signal anchors it. It does not contradict the canonical reference: the reference is silent at that position. This is why the five variance manifestations do not catch it, and why it has its own — the **unanchored assertion**.

**Probable cause:** A position a reader expects to be filled is declared nowhere in the corpus. Silence is not neutral in a probabilistic system — it is an invitation to fill.

**Typed correction:**
- Occupy the position editorially — declare the value, or close the set by declaring that none applies. The closure clause is the same instrument as under Projection; what differs is only that the closed attribute is established nowhere rather than elsewhere
- Reinforce declaratively — the declarative signal files carry the same declaration in machine-readable format, after the corpus carries it, never instead of it
- Do not treat as a projection — displacement has nothing to displace here. A correction aimed at pushing the attribute away leaves the position empty, and an empty position is filled again

**Priority:** 1 bis. Treated in parallel with priority 1.

---

## Correction matrix

| Operation | Diagnostic question | Correction |
|---|---|---|
| Generalization | Category instead of expertise? | Densify central concept + reduce peripheral weight |
| Amalgamation | Merged with competitors? | Reinforce proprietary concepts + exclude shared terms |
| Truncation | Correct but incomplete? | Reinforce obligatory associations between components |
| Substitution | Proprietary term replaced? | Exclude generic + densify proprietary + contrastive associations |
| Projection | Category properties attributed? | Densify real signal + close the set editorially + declare in sio-corrections.json |
| Inferential filling | Unaddressed question answered? | Occupy the position: close the set editorially, then reinforce declaratively |

---

## Priority matrix

| Priority | Type | Operations | Principle |
|---|---|---|---|
| 1 | Identity loss | Amalgamation, Substitution | Without distinct identity, nothing else matters |
| 2 | Identity distortion | Generalization | Signal present but distorted |
| 3 | Incomplete signal | Truncation | Signal present but amputated |
| 4 | Polluted signal | Projection | Noise added, not signal lost |
| 1 bis | Manufactured signal | Inferential filling | Outside the dependency chain; nothing argues for deferring it |

Structural principle: **loss → distortion → incompleteness → pollution.**  
Restore what disappeared. Correct what is distorted. Complete what was amputated. Clean what was added.

Inferential filling sits outside that sequence because the sequence orders by dependency, not by severity. Occupying a position neither requires a prior correction nor blocks one: the position carries no competing declaration to displace first.

---

## Limits

Typed correction does not guarantee reconstruction correction. The box remains opaque. The model remains probabilistic. Correction is an intervention on inputs whose effect on outputs is observable but not guaranteed.

Typed correction does not produce immediate effects. Latency between corrective signal injection and integration in reconstructions varies by model, update cycle, and retrieval mechanism. Latency is structural, not accidental.

Some distortions resist endogenous correction because their cause is primarily exogenous — a competing signal massively denser in the global interpretive space. In these cases, typed correction reduces the distortion without eliminating it. Recognizing this limit is part of the discipline.

Typed correction requires prior diagnosis — a systematic inferential audit that identifies not only that reconstruction is distorted, but which type of distortion is active. Without diagnosis, correction remains generic. And generic correction in a probabilistic system is random correction.

**Typed correction is inferential governance applied. Not control. A structured, repeatable intervention whose effect is observable but not guaranteed — in a system no one controls.**

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
- [Declarative Hub](https://github.com/MMaquet/signal-inference-optimization/blob/main/declarative-hub.md)
- [Technical Foundations](https://github.com/MMaquet/signal-inference-optimization/blob/main/technical-foundations.md)
- [Article series](https://medium.com/@melaniemaquet)

**First public commit:** April 18, 2026  
**Version:** 1.3  
**Last updated:** October 31, 2026  
**Author:** Mélanie Maquet — SEMANTIKIA
