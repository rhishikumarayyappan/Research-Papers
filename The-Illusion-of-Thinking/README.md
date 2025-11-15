# Reasoning Collapse Simulator — Multi-Puzzle Research Toolkit

**Author:** Rhishi Kumar Ayyappan

---

## Project Overview

**Research Challenge:**  
Understanding the limitations of step-by-step reasoning in current algorithms and humans is critical for advancing AI safety, reliability, and capability. Classic puzzles such as Tower of Hanoi, Blocks World, River Crossing, and Checker Jumping provide a precise environment to empirically measure where, why, and how reasoning collapses as complexity increases. This toolkit brings the theory and evidence from *The Illusion of Thinking* into practice for research, teaching, and AI portfolio-building.

---

## Key Achievements & Metrics

- **Multi-Puzzle Coverage:**  
  - Modular, fully implemented simulators for Tower of Hanoi, Blocks World (arbitrary stacks), River Crossing, and Checker Jumping.
- **Automated Collapse Detection:**  
  - Collapse points identified via solution attempts, validated against theoretical minimum steps, with instant flags for unsolved or inefficient reasoning.
- **Rich Visualizations:**  
  - Includes `reasoning_collapse.png`  
    *Sample chart below shows solution steps vs. complexity across all puzzles, with visible collapse points.*

  ![Reasoning Collapse Across Puzzles](reasoning_collapse.png)
- **Annotated Replay:**  
  - Stepwise chain-of-thought replays for all puzzles, diagnosing incorrect or inefficient reasoning and making failure transparent.
- **Metrics Table Sample:**

  | Puzzle        | Complexity | Steps | Overthinking | Failure At Step | Solved |
  |---------------|------------|-------|--------------|-----------------|--------|
  | Hanoi         | 2          | 3     | False        | —               | True   |
  | Hanoi         | 6          | 0     | False        | —               | False  |
  | BlocksWorld   | 5          | 5     | False        | 5               | False  |
  | RiverCrossing | 4          | 7     | False        | —               | True   |
  | CheckerJump   | 4          | 0     | False        | —               | False  |

---

## Methods Used

- **Puzzle Simulators:**  
  Clean, extensible Python classes for each environment, with move validation, replay, and history tracking.
- **Diagnostics & Replay:**  
  Automated failure and overthinking detection; reasoning traces are replayed and annotated in both the table and visual outputs.
- **Visualization:**  
  Matplotlib and Seaborn for instant dashboard creation.
- **Manual/Agent Mode:**  
  User, scripted, and future agent/LLM reasoning supported for side-by-side comparison.

---

## Business & Research Impact

- **AI Safety & Reliability:**  
  Empirical diagnosis of reasoning collapse points helps improve model robustness and understand limits—a key challenge in LLM reliability.
- **Education & Teaching:**  
  Interactive notebook and replay mode make it ideal for classroom demonstrations or interview challenges.
- **Human vs. Algorithm Benchmarking:**  
  Enables direct comparison of human chains-of-thought vs. scripted and algorithmic approaches, supporting cognitive science and AI benchmarks.
- **Portfolio/Recruiter Value:**  
  Ready-to-show visual analytics, clean diagnostics, and modular code stand out in interviews and research submissions.

---

## Visuals

- **Reasoning Collapse Dashboard:**  
  (reasoning_collapse.png)  
  *Demonstrates sharp collapse points and reasoning efficiency across classic puzzles.*

- **Reasoning Trace Replay:**  
  *Solution traces and failure diagnostics displayed for any puzzle at any step.*

---

## How to Run

1. **Clone the repository:**
