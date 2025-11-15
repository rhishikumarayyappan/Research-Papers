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
<img width="851" height="479" alt="reasoning_collapse" src="https://github.com/user-attachments/assets/f8e96454-c841-4159-b3d6-51678983e929" />

  *Demonstrates sharp collapse points and reasoning efficiency across classic puzzles.*

- **Reasoning Trace Replay:**  
  *Solution traces and failure diagnostics displayed for any puzzle at any step.*

---

## How to Run

1. **Clone the repository:**

git clone https://github.com/rhishikumarayyappan/Reasoning-Collapse-Simulator.git

cd Reasoning-Collapse-Simulator


2. **Install requirements:**
pip install matplotlib seaborn pandas numpy


*(Or use the provided requirements.txt file)*

3. **Launch the notebook:**
jupyter notebook Reasoning_Collapse_Simulator.ipynb


Or simply use Google Colab for easy execution with instant visual outputs.

4. **Run all cells (Runtime → Run all):**
- All puzzle environments are set up, replay and diagnostics enabled by default.
- Visuals, metrics, and reasoning replays are generated automatically for every test.

---

## Tech Stack

- Python
- Matplotlib & Seaborn
- Pandas & NumPy
- Google Colab/Jupyter Notebook

---

## For Full Implementation & Research Insights

- See the included notebook for all puzzle classes, replay logic, complexity ramp demos, and side-by-side comparisons.
- Contributions welcome—add new puzzles, agent modes, or analytics for even deeper reasoning diagnostics.

---

**Questions? Interested in collaborating or benchmarking new AI agents? See the FAQ section in the notebook, or open an issue in the repository!**

---

*Visual file: `reasoning_collapse.png` should be placed in your repo and properly referenced in the README for best recruiter/researcher impact.*
