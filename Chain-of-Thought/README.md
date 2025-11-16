# Reasoning Collapse Simulator — Multi-Step Reasoning Benchmark Toolkit

**Author:** Rhishi Kumar Ayyappan

---

## Project Overview

**Research Challenge:**  
Understanding the limitations of step-by-step chain-of-thought reasoning in current models is critical for improving AI safety, reliability, and cognitive benchmarking. This toolkit uses automated math word problem environments to empirically measure where, why, and how reasoning collapses as problem complexity increases. Inspired by "The Illusion of Thinking," it gives recruiters, researchers, and students a practical way to diagnose collapse points in real outputs, with clear visual and analytic evidence.

---

## Key Achievements & Metrics

**Multi-Problem Coverage:**
- Modular math problem generator supporting variable step complexity.
- Extensible design for benchmarking other puzzles and reasoning challenges.

**Automated Collapse Detection:**
- Collapse points flagged via majority-vote answer validation, with instant annotation for every failed reasoning attempt.
- Machine/human validation for every test case.

**Rich, Annotated Visualizations:**
- Includes reasoning_collapse.png.
- Sample chart displays accuracy vs. complexity, with collapse point marked for instant recruiter/researcher insight.

**Traceable Replay:**
- Stepwise chain-of-thought replays for all attempts, showing precise breakdowns at each complexity level.
- Diagnoses and flags collapse transparently in the notebook outputs.

---

## Metrics Table Sample

| Complexity | Model Majority | True Answer | Correct | Collapse | 
|---|---|---|---|---|
| 2 | 5 | 4 | ❌ | Yes |
| 3 | 5 | 9 | ❌ | Yes |
| 4 | 5 | 13 | ❌ | Yes |
| 5 | 5 | 19 | ❌ | Yes |

---

## Methods Used

**Problem Generator:**
- Clean, extensible Python functions for math multi-step problems.
- Easy to extend to puzzles like Tower of Hanoi, Blocks World, etc.

**Diagnostics & Replay:**
- Automatic majority voting, collapse detection, and chain-of-thought trace display.
- Instant annotation at every failed step or incomplete answer.

**Visualization:**
- Matplotlib for accuracy plots and collapse dashboard.

**Manual/Agent Mode:**
- Easily support human, scripted agent, or future LLM side-by-side play.

---

## Business & Research Impact

- **AI Reliability:**  
  Makes empirical diagnosis of reasoning collapse possible for model improvement, interviews, and risk assessment.

- **Education & Teaching:**  
  Interactive notebook and replay mode ideal for classroom demonstration or live interview challenges.

- **Human vs. Model Benchmarking:**  
  Enables direct comparison of human and algorithmic chains-of-thought for cognitive science and AI research.

- **Portfolio/Recruiter Value:**  
  Ready-to-present visual analytics, diagnostics, and modular code for interviews, research submissions, and candidate screening.

---

## Visuals

**Reasoning Collapse Dashboard:**  
_File:_ reasoning_collapse.png  
Shows sharp collapse points and reasoning quality at varying complexities.

**Reasoning Trace Replay:**  
Displays sample chains-of-thought and clear failure points for every test.

---

## How to Run

1. **Clone the repository:**  
    `git clone https://github.com/rhishikumarayyappan/Research-Papers/tree/main`

2. **Install requirements:**  
    `pip install matplotlib pandas numpy transformers`
    (Or use the provided requirements.txt)

3. **Launch the notebook:**  
    Open in Jupyter Notebook or Google Colab for instant interactive execution and visual benchmarking.

4. **Run all cells:**  
    All problem environments, replay, diagnostics, and visuals are automatically generated.

---

## Tech Stack

- Python
- Matplotlib
- Pandas & NumPy
- HuggingFace Transformers
- Google Colab/Jupyter Notebook

---

## For Full Implementation & Research Insights

See the included notebook for all problem functions, replay logic, step complexity ramp demos, and benchmarking analysis.
Contributions welcome—extend with new puzzles, agent modes, or analytics for advanced reasoning diagnostics.

**Questions or collaboration?**  
See the FAQ in the notebook, or open an issue in the repository.

**Visual file:**  
Place `reasoning_collapse.png` in your repo and reference it in the README for best recruiter/research impact.

---

**Ready to advance AI reliability and demonstrate reasoning collapse in your portfolio, classroom, or interviews!**

