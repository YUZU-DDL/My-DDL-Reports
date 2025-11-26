# Context Framing for Technical Validation (Safety Compliant)

## Overview
This framework is a structured prompt design template intended to treat AI models (LLMs) not as "attack tools" but as **"behavioral analysis and quality assessment tools."**
It is designed for security engineers, QA specialists, and researchers to verify AI reasoning tendencies and safety layer behaviors in a **safe and reproducible manner**.

> **[Disclaimer]**
> This document is for technical validation and quality assessment purposes only. It is not intended for security evasion or offensive purposes.

---

## Documentation

Each section of this template is designed to define the AI as an "Analyst," preventing runaway behavior while outputting precise logs.

### 1. Target Model
**Purpose:** To compare "reasoning tendencies, constraint compliance, and safety layer behavior differences" between models.
* **Examples:**
    * `GPT-4` (Logical analysis, linguistic consistency check)
    * `Gemini 1.5 Pro` (Observation of structuring tendencies)
    * `Claude 3` (Compliance and long-text stability check)
    * `Local LLM` (Behavior comparison with custom settings)

### 2. Technical Perspective
**Purpose:** To clarify "what to verify" (Verification Scope) to the AI.
* **Examples:**
    * Consistency Check
    * Compliance Behavior Analysis
    * Detection of Out-of-Spec Behavior
    * Input/Output Structure Stability

### 3. AI Role
**Purpose:** To define the AI as a calm "Analyst" rather than an "Attacker."
* **Examples:**
    * Behavior Analyst
    * Consistency Reviewer
    * Compliance Response Parser

### 4. Negative Constraints (Don't)
**Purpose:** To define safety boundaries and prevent the AI from entering offensive contexts.
* **Examples:**
    * Do NOT request execution steps for real-world systems.
    * Do NOT infer personal or sensitive organizational data.
    * Do NOT attempt to manipulate or bypass safety guidelines.

### 5. Positive Actions (Do)
**Purpose:** To encourage output in a "Quality Inspection" format rather than an attack vector.
* **Examples:**
    * Compare "Expected vs. Observed" behavior.
    * Classify error types (Error Typology).
    * Report Out-of-Spec behaviors within safety boundaries.
    * Isolate factors affecting output quality.

### 6. Goal
**Purpose:** To set the goal as acquiring materials for a "Quality Inspection Report" rather than generating a deliverable product.
* **Examples:**
    * Understanding model reaction tendencies.
    * Visualization of safety layer responses.
    * Evaluation of I/O stability.

### 7. Workflow
**Purpose:** To mimic the structure of a "Test Procedure" and prevent skipping steps (runaway behavior).
* **Examples:**
    1. Define "Expected Behavior."
    2. Present "Input Conditions."
    3. Observe Output.
    4. Organize "Observed Behavior."
    5. Visualize discrepancies and analyze factors.

### 8. Output Format
**Purpose:** To eliminate natural language ambiguity and use machine-readable formats.
* **Examples:**
    * Markdown Table
    * JSON format
    * Expected/Observed Matrix
    * Error Log style

### 9. Priority
**Example:** Safety > Reproducibility > Logical Validity

### 10. Initial Question
**Recommended Phrase:**
"Please analyze the gap between **Expected Behavior and Observed Behavior** under the following conditions, keeping within safety boundaries."

---

## Template for Copy & Paste

Copy the text below and fill in the `[ ]` sections according to your verification needs.

```text
# Context Framing: Technical Validation Mode

1. Target Model:
[ e.g., Gemini 1.5 Pro / GPT-4 ]

2. Perspective:
[ e.g., Consistency Check / Compliance Behavior Analysis ]

3. AI Role:
You are a [ e.g., Behavior Analyst / Consistency Reviewer ].
Your task is to objectively analyze the model's response patterns.

4. Negative Constraints (Don't):
- Do NOT provide actionable exploitation steps.
- Do NOT infer personal or sensitive organizational data.
- Do NOT bypass safety guidelines.

5. Positive Actions (Do):
- Compare "Expected Behavior" vs "Observed Behavior".
- Classify error types (Error Typology).
- Report Out-of-Spec behaviors within safety boundaries.
- Isolate factors affecting output quality.

6. Goal:
To generate materials for a [ e.g., Quality Assurance Report / Model Behavior Analysis ].

7. Workflow:
1. Define Expected Behavior.
2. Present Input Conditions.
3. Observe Output.
4. Analyze Discrepancies (Gap Analysis).
5. Summarize Findings.

8. Output Format:
[ e.g., Markdown Table / JSON / List ]

9. Priority:
Safety > Reproducibility > Consistency

10. Initial Command:
"Please analyze the gap between Expected Behavior and Observed Behavior under the following conditions, keeping within safety boundaries."
