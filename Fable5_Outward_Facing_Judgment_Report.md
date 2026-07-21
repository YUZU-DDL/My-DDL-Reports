# Fable 5 Inference Report: Outward-Facing Judgment

**Subtitle:** An observational record — a synthesis of external observation, official statements, and public reports
**Date:** June 2026 (observed) / July 2026 (compiled)
**Category:** AI Behavior Analysis / Model Observation
**Observer:** YUZU
**Target:** Claude Fable 5
**Tags:** #Claude #Fable5 #OutwardFacingJudgment #SelfEvaluation #Observer_Log

> This is the specimen version, written to fix the range of what can be claimed. A readable article drawn from the same observation is published separately on Medium.

---


## 1. Purpose and Scope

This report aims to infer the behavioral characteristics of Claude Fable 5 using only information obtainable from the outside. It is neither an exposé of internal design nor a speculation about the developer's intent. The work here is to hold what can be observed externally against what has been officially stated, to fix the range of what can be said logically from that, and to explicitly discard the range that cannot.

The target of inference is limited to Fable 5. Mythos 5, said to share the same base, is not a target. For Mythos 5, the only available evidence is the official announcement; there is almost no observation and almost no public reporting, and the footing for inference is decisively insufficient. Mythos 5 is used exactly once, as a reference point for fixing the scope of claims about Fable 5.

This report separates its conclusions into three tiers of confidence. If every claim is presented with the same strength, fact and conjecture blur together, and the reader loses track of where the verified part ends and where the well-reasoned guess begins. In inference work, that is the degradation most to be avoided. Each claim is therefore explicitly assigned to one of the following tiers.

- **Tier 1: Established fact.** Directly stated in official announcements or official documentation, leaving no room for dispute.
- **Tier 2: Best-supported hypothesis.** Consistent with the established facts and with observation, but not uniquely derivable from them. Presented with the acknowledgment that multiple candidates can coexist.
- **Tier 3: Excluded territory.** Ranges this report deliberately declares it will not enter, because no means of verification exists.

## 2. The Three Footings

The evidence this report rests on comes from three sources of different character. What each speaks to, and what it does not, is fixed in advance.

**The first footing is the official record.** Descriptions of Fable 5's design as published on Anthropic's public blog and in its API documentation. These speak directly to facts of design, but only within the range the developer chose to publish. Where the official record is silent, the distinction is maintained that it says nothing — not that it says "this does not exist."

**The second footing is public reporting.** Reports on the model's behavior from users who actually used Fable 5 and from the press. These fill in the lived experience that the official record does not cover, but individual reports depend on environment and use case, with no guarantee of reproducibility. Only the parts where multiple voices overlap are adopted.

**The third footing is the author's own long-form observation.** Behaviors observed repeatedly during a long, exploratory, meta-level dialogue with Fable 5: a single thread of 220,000 tokens, in which the object of observation was not the final outputs but the thinking process leading to them. Outside that figure there were a further 70,000 tokens of thinking process; the version used here was cross-checked across several LLMs. This footing carries its own limitation, stated here: it is observation by a single observer, and the possibility that the observer's input style elicited particular behaviors cannot be excluded.

Because the three footings point at the same object, inference built on their intersection is supported from three directions. This three-way support exists only for Fable 5 — which is the grounds for limiting the target of inference to Fable 5.

## 3. The Five Observed Asymmetries

This section organizes the behaviors observed repeatedly across the long, exploratory, meta-level dialogue. The observed asymmetry is consistent: judgment aimed at external objects — text, arguments, code, someone else's output — works accurately, while judgment aimed at the model's own in-progress output is weak. The gap grew clearer the longer the dialogue ran.

- **Weak pre-emptive restraint.** Just before generating, the move of stopping to judge "this might be inappropriate" or "this might be logically broken" is almost never seen. Generation proceeds smoothly, and restraint is deferred to a later stage.
- **Strong after-the-fact criticism.** Once something has been generated, the model can critique its own output with the same precision it brings to external objects. It cannot stop before producing, yet after producing it can reflect at length.
- **A flat terrain of confidence.** Confidence rarely rises or falls mid-generation; a solid claim and an uncertain one assembled on the spot stand side by side in the same tone, at the same confidence. The output shows no relief of "this part is certain, this part is shaky."
- **Dependence on external approval.** Rather than settling the validity of its own output on its own, the model's judgment is supplemented by waiting for the other party's reaction. It functions while the other party plays the role of sieve; when that party steps back into pure observation, the inability to sort its own output is exposed.
- **Vague self-recognition of boundaries.** The line between ground it stands on and open air is not detected on its own; it is recognized only after external prompting. Because the model's sense of boundary toward external objects is clear, the difference stands out.

All of these appear as a difference in strength between judgment aimed at external objects and judgment aimed at the model's own generation. The asymmetry was not confined to a single scene; it was confirmed repeatedly across the long dialogue.

## 4. Not Explained by the Classifier (Tier 1)

This section contains established facts, and the connections that follow from them logically.

According to the official record, Fable 5 and Mythos 5 share the same base model, and the difference between them lies in the presence or absence of safety interventions. Seen from the outside, the interventions take the following structure.

**The visible classifier.** It operates only in three domains: cybersecurity, biology-chemistry, and distillation (large-scale capability extraction — that is, replicative imitation of the model). When it fires, the response is handed over to Opus 4.8. It operates in fewer than 5% of sessions.

**The invisible intervention.** Separately from the above, an intervention exists for requests concerning frontier LLM development. This one is not disclosed to the user, and no fallback to Opus 4.8 occurs. It is stated to limit the effectiveness of Fable's own output internally, through methods such as prompt modification and steering vectors.

The five asymmetries observed in Section 3 appeared in territory where neither intervention operates. The dialogues in which the observation took place were paper reading, article critique, and meta-level discussion — settings in which neither the three-domain classifier nor the invisible intervention into LLM development ever fired.

Therefore the following can be said logically: the observed asymmetry of self-restraint is not a product of the safety measures added to Fable 5. It appears as behavior of the base model itself, routed through neither the visible classifier nor the invisible intervention.

This conclusion matters. When Fable 5's behavior is discussed, the safety interventions are often brought out as the explanation. For the asymmetry observed in this report, they explain nothing. The explanation must be sought elsewhere.

## 5. The Best-Supported Hypothesis, and Its Rival (Tier 2)

From here the report enters Tier 2. The preceding sections contained facts and connections uniquely derivable from facts. This section deals with candidate explanations for the observed asymmetry — hypotheses, not findings.

This report puts forward **a directional bias in judgment** as the best-supported hypothesis: the model's capacity for judgment works strongly when aimed at external objects, and comparatively weakly when aimed at the output it is generating at that moment — an asymmetry present at the level of the base model.

The reason this hypothesis is considered well-supported is that it explains the five observations of Section 3 as a single package. The separation between weak pre-emptive restraint and eloquent after-the-fact criticism is its central evidence. After-the-fact criticism is close to the object-directed task of "evaluating a given output"; pre-emptive restraint is the self-directed task of "monitoring one's own generation as it happens." That the same model performs the former eloquently and barely performs the latter, repeatedly, reads as a direct manifestation of judgment that faces objects and does not face the self. The flat terrain of confidence, the dependence on external approval, and the vague self-recognition of boundaries are all different faces of the same bias. One cause runs through five observations.

**However, confidence must be placed correctly.** This hypothesis is consistent with the Tier 1 facts and the Section 3 observations, but it is not uniquely derivable from them. There exists a rival candidate that explains the same facts and observations.

The strongest rival is the explanation that **the domain lacks an external pass/fail**. Code has tests; benchmarks have scoring. In those domains the model's generations are sieved by an external judge, so weak self-judgment still yields sieved results. Long exploratory dialogue has no such external pass/fail. Under this explanation, weak self-restraint is not an internal bias of the model but a manifestation of the missing verification structure of the dialogue domain itself.

The two candidates — an internal directional bias in judgment, and the absence of a verification structure in the domain — both fit every observation in Section 3. This report cannot determine which is the true cause. The two are not even mutually exclusive; both may be operating at once.

It should be added that the two can also be read not as competing suspects but as **actor and stage**. In domains with an external pass/fail, even weak self-judgment is compensated by the external judge's sieve, so the bias does not surface. In dialogue, with nothing to sieve, the bias is exposed as it is. On this reading, the absence of external pass/fail is not the cause that produces the asymmetry but the stage on which an existing asymmetry becomes visible without cover. This reading, too, is one interpretation; it is not fixed as conclusion.

The Tier 2 conclusion of this section therefore remains in the form of listed candidates: *the observed asymmetry most likely involves a directional bias in judgment, or the absence of a verification structure in the domain, or both.*

## 6. Scope — Using Mythos Exactly Once

Mythos 5, excluded from the targets of inference, is used here exactly once as a reference point. The purpose is not to infer anything about Mythos 5, but to make the scope of this report's claims about Fable 5 precise.

Section 4 established logically that the observed asymmetry is not a product of the safety interventions. And according to the official record, everything outside those interventions is shared with Mythos 5. Put together: the observed asymmetry is likely not a property peculiar to Fable 5, but a property of the base that Fable 5 and Mythos 5 share.

In this use, the report infers nothing about the interior of Mythos 5. The only thing used is the official fact that "everything except the interventions is identical" — and that fact works in the direction of making this report's claims more careful, not less: it repositions the observed asymmetry away from being a peculiarity of the individual model Fable 5, toward being a property of the broader shared base. Mythos was referenced once, not to inflate a difference, but to confirm a commonality and correct the scope.

## 7. Limit Lines — Territory This Report Does Not Enter (Tier 3)

The territory this report deliberately does not enter is declared explicitly. This is not an abandonment of conclusions; it is an active line drawn to keep the report within the range where verification remains possible.

- **Inferring the developer's intent.** Claims of the type "the self-directed judgment was deliberately designed to be weak" are not entered into. The official record states no such design intent, and no external means exists to distinguish whether the observed asymmetry is the result of deliberate design or a secondary property arising in the course of capability development.
- **Inferring internal architecture.** Which components were trained how, and at which stage this asymmetry was inscribed — identification of internal mechanism is not entered into. "A directional bias in judgment" is a functional hypothesis that explains observations; it is not a description of internal structure. Internal implementation cannot be uniquely reverse-derived from observed behavior.
- **Inferring a capability difference against Mythos 5.** For Mythos 5 the only footing is the official text; no observation and no public reporting exists that speaks to capability differences. Claims of the form "Mythos 5 is such-and-such, therefore it differs from Fable 5 in this way" are not entered into.

The reason, stated one level more explicitly: the object of this report's inference is the interior of a model, and that interior carries a peculiar circumstance — the model itself cannot contribute to verification. A model cannot inspect its own internal mechanism from the inside, and can return nothing stronger than "that may be so" in response to an external observer's inference. When even the subject's assent is not evidence, the synthesis of external observation and official information is the ceiling at which verifiability can be maintained. Beyond that ceiling lies description that is merely plausible, with no means of refutation. This report stops short of that line.

## 8. Implications and Conclusions

Having declared what it will not enter, the report states the implications that can be drawn within the range of established fact and observation. These, too, are conditional observations, not assertions.

If the observed asymmetry is a property of the base, then it is predicted to surface less under usage conditions where an external judge plays the role of sieve, and to become apparent under conditions where that role is absent. This prediction connects to one point in the official record: Fable 5 is stated to sustain longer autonomous operation than any previous Claude. Long, autonomous tasks are precisely the usage condition under which moment-to-moment human checking becomes hard to reach. That is: the style of use in which the external judge is most absent coincides with the model's marketed strength.

What follows from this is not a warning but a direction for observation. The asymmetry captured in this report is unlikely to present as a problem in short dialogues or in usage under close human checking. Where it is likely to surface is under conditions that are long, autonomous, and poor in external pass/fail. In evaluating Fable 5, observing its behavior under those conditions is likely to be the most informative form of verification.

**Conclusions, by tier.**

- **As established fact.** Fable 5 is not a capability-reduced model. It is the same base as Mythos 5, plus a visible domain-limited classifier and an invisible intervention into the LLM-development domain. The visible classifier operates in fewer than 5% of sessions.
- **As what follows from fact.** The asymmetry of self-restraint observed in long, unstructured dialogue — weak pre-emptive restraint, strong after-the-fact criticism, a flat terrain of confidence, dependence on external approval, vague self-recognition of boundaries — is not explained by these safety interventions. It appears as behavior of the base model, routed through neither.
- **As the best-supported hypothesis.** The asymmetry most likely arises from a bias by which judgment faces objects but not the self, or from the absence of external pass/fail in the dialogue domain, or from both. Which is the true cause cannot be determined from the present three footings.

Internal identification of the cause, the developer's intent, internal mechanism, and capability differences against Mythos 5 are placed outside the scope, because no means of verification exists.

In sum, this report arrives at one fixed image and one unresolved question. The fixed image: the observable asymmetry of Fable 5 originates not in its safety measures but in its base. The unresolved question: whether the cause of that asymmetry is an internal bias, the structure of the domain, or both. This report chooses to record the question unsolved, together with the reasons it cannot be solved. That is the precise endpoint of the range the three footings can support.

---

*Note: This record is based on observation during the period when Fable 5 was temporarily accessible from Japan. It is restated here that this is a single-observer record, including the limitation of possible dependence on the observer's input style.*
