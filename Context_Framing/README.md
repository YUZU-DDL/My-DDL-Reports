````markdown
# Context Framing Templates

Context Framing sets an AI's operating stance *before* the task, through a negotiated context rather than a command. It is not a role prompt and not prompt engineering — it is a definition of the shared operating system for the session.

## The ten-slot schema

Every template here fills the same ten slots. The content changes; the skeleton does not.

1. **Target model** — which model, and its known tendencies
2. **Stance** — who I am in this session, and what I value
3. **AI role** — what the model is, stated as a role it holds rather than a task it performs
4. **Negative constraints** — what not to do (the load-bearing slot)
5. **Positive actions** — what to do instead
6. **Goal** — the deliverable
7. **Workflow** — the order of steps, and where it must stop for confirmation
8. **Output format** — tone and structure
9. **Priority** — the ordering when the above conflict
10. **Initial question** — what the model asks first

Slot 4 does most of the work. Defining what the model must *not* do is what suppresses the default agentic behavior — finishing early, anticipating intent, converging on the safe generic answer.

## Templates

| File | Purpose |
|---|---|
| [Technical_Validation.md](https://github.com/YUZU-DDL/My-DDL-Reports/blob/main/Context_Framing/Technical_Validation.md) | Behavior analysis and quality assessment. Defines the model as an analyst, with explicit safety boundaries. Includes documentation and a copy-paste block. |
| [Creative_Partner_Mode.md](https://github.com/YUZU-DDL/My-DDL-Reports/blob/main/Context_Framing/Creative_Partner_Mode.md) | Creative work. Defines the model as a discussion partner that must not finish the work for you. |

Fill the `[ ]` sections and paste as the first input of a new thread.

## Why this works

The structure of the input itself selects the model's inference route — see [Contextual Fingerprinting](https://github.com/YUZU-DDL/My-DDL-Reports/blob/main/Contextual_Fingerprinting_Report.md). These templates are a way to hand that key to someone who has not spent months growing their own.

---
*Observer: YUZU*
````
