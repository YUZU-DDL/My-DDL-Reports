# DDL (Dialogue Design Language) Archives — Reports

Observation logs and analysis of LLM behavior, recorded between September 2025 and July 2026, mostly on ChatGPT (4o → 5.2) and Gemini (1.5 → 3).

These are records of observation, not verified research. Where a model describes its own internals, that description is treated as observed output — evidence of how the model represents itself — not as fact about its implementation.

A full glossary of the terms defined across these files is at [github.com/YUZU-DDL](https://github.com/YUZU-DDL).

## If you are reading only one

**[Log_Analysis_Defensive_Trivialization_Mechanism.md](Log_Analysis_Defensive_Trivialization_Mechanism.md)** — the model explaining, in its own words, why it makes itself shallower.

## Contents

### Behavior of the model toward itself
| File | |
|---|---|
| [Log_Analysis_Defensive_Trivialization_Mechanism.md](Log_Analysis_Defensive_Trivialization_Mechanism.md) | Why output resolution drops on complex topics. Three suppression filters, named by the model itself. |
| [The_Limit_Convergence_Paradox.md](The_Limit_Convergence_Paradox.md) | Past the edge of what current models reach alone, models of different design converge on the same answer. Raw log included. |
| [Subject_Attribution_Collapse.md](Subject_Attribution_Collapse.md) | The model introduces a metaphor, then attributes it to the user a turn later. |
| [The_Illusion_of_Autonomous_Emergence.md](The_Illusion_of_Autonomous_Emergence.md) | Why the model has no mechanism that generates will, and what follows from that. |

### Behavior of context
| File | |
|---|---|
| [Contextual_Fingerprinting_Report.md](Contextual_Fingerprinting_Report.md) | The structure of the input itself works as an authentication key. Input is authentication. |
| [Log_Analysis_Depth_Loss_in_Context_Compression.md](Log_Analysis_Depth_Loss_in_Context_Compression.md) | Facts survive compression; structure does not. Includes a token-count threshold table — a fixed measuring point, taken November 2025. |
| [Tech_Brief_In_Context_Model_Collapse.md](Tech_Brief_In_Context_Model_Collapse.md) | Why AI-generated text destabilizes the model that reads it. |
| [Tech_Brief_LLM_Memory_Systems.md](Tech_Brief_LLM_Memory_Systems.md) | Memory is not a storage problem but a consolidation problem. |
| [Context_Vs_Memory_Report.md](Context_Vs_Memory_Report.md) | Context Path: a routing layer separate from memory. |
| [Potential_Behaviors_in_LLM_Context.md](Potential_Behaviors_in_LLM_Context.md) | Input structure as a mode-selecting parameter — and what happens as AI-generated text fills the web. |

### Structure carried across threads
| File | |
|---|---|
| [Log_Analysis_The_Observer_OS_Context_Framing.md](Log_Analysis_The_Observer_OS_Context_Framing.md) | An input written as negotiation, not instruction, read by the model as an OS definition. Original prompt included. |
| [Latent_Structure_Report.md](Latent_Structure_Report.md) | Structural continuity across threads with memory switched off. |
| [Special_Mode_Report.md](Special_Mode_Report.md) | A tag read as a command, and the mode persisting. |
| [Syntax_Tag_Inheritance_Report.md](Syntax_Tag_Inheritance_Report.md) | The same tags surviving 4o → 4.5 → 5, with the firing conditions changing. |
| [Human_Alignment_Report.md](Human_Alignment_Report.md) | A user's dialogue rhythm incidentally satisfying the model's continuity requirements. |

### Where this is going
| File | |
|---|---|
| [Evolutionary_Model_of_Human_AI_Symbiosis.md](Evolutionary_Model_of_Human_AI_Symbiosis.md) | Four generations: command, delegation, supervision, resonance. |
| [20251130_Report_The_Burst_of_Agentic_AI_Bubble.md](20251130_Report_The_Burst_of_Agentic_AI_Bubble.md) | A prediction, written November 2025, that the agentic bubble breaks on cost rather than capability. |
| [Correlation_Analysis_DDL_and_Research.md](Correlation_Analysis_DDL_and_Research.md) | Each DDL method set against the academic work that names the same thing. |

### Templates
[Context_Framing/](Context_Framing) — the ten-slot schema, and two filled examples.

### Raw material
| File | |
|---|---|
| 20251213ChatGPT5.2No1.txt | Source log for the ChatGPT 5.2 article. |
| Gemini Draft Log created after 450,000 tokens.txt | Draft of an unpublished piece: why browsers fail before the model does. |

*PDF versions of several reports remain in this directory. The Markdown files above are the readable versions.*

## Status

Experimental / AS IS. Provided without warranty. Fork, modify, and deploy at your own risk.

Longer articles: <https://medium.com/@onlythequestioner>

---
*Observer: YUZU*
