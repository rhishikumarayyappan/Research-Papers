# Difficulty-Adaptive Reasoning & Collapse Diagnostic Simulator

**Author:** Rhishi Kumar Ayyappan

---

## Project Metrics

| Difficulty | #Problems | Correct (%) | Avg Tokens Used | Collapse Flags (%) |
|------------|-----------|-------------|-----------------|--------------------|
| Easy       |     2     |      0      |     62          |        100         |
| Medium     |     2     |      0      |     67          |        100         |
| Hard       |     1     |      0      |     79          |        100         |

- **Tokens Used:** Models consume about 60-80 tokens per answer regardless of difficulty, signaling overthinking even when a simple response would do.
- **Collapse Rate:** 100% for all tested samples, showing that current open/free models do not handle adaptive reasoning or complexity increases well.

---

## Visualisation

<img width="989" height="490" alt="token_accuracy_adaptive_difficulty" src="https://github.com/user-attachments/assets/93d38a58-c006-4cba-9ccd-265c989cd8cc" />


- **Token Use:** Flat across all difficulties, not adaptive—models waste compute on easy tasks.
- **Accuracy:** Model fails to get correct answers at any difficulty in tested examples.
- **Red Line Indicator:** Shows "overthinking threshold"—over-budget responses flagged automatically.

---

## Business Impact

- **Efficiency Diagnostics:** Quickly shows if models are wasting cloud budget or API calls on long answers; helps teams design better benchmarks and save cost.
- **Reliability Flags:** Collapse detection spots where models are likely to give wrong answers, making it easy to set up fallback or review logic in production.
- **Hiring & Portfolio Value:** Demonstrates modern benchmarking methods for reasoning collapse, efficiency, and chain-of-thought diagnostics—ideal for candidate interviews, technical vetting, or AI risk reviews.
- **Team & Stakeholder Clarity:** Outputs, charts, and badges make performance and failure easy for anyone to read, discuss, and act on.

---

## Ready-to-Present Summary

- This project uses open/free models to recreate the findings of cutting-edge AI research on reasoning collapse and adaptive efficiency.
- Visualizes when and why models break down, and how hard it is to reliably budget reasoning in practice.
- Provides both technical and business evidence for the need for smarter, more adaptive AI strategies—and the limits of current approaches.

---


