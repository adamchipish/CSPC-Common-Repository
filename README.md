# CSPC — Computer Science for Physics and Chemistry

My coursework repository for the course.
Each practical lives under `PW<n>/Lab <X>/`.

## Setup

Create and activate the environment for a given lab:

```bash
conda env create -f "PW<n>/Lab <X>/environment.yml"
conda activate cspc
```

Run the tests for a lab from inside its folder:

```bash
cd "PW<n>/Lab <X>"
pytest -v
```

---

## PW1 — Lab A: Reproducible Foundations

**What I built:**
- <one or two lines: the CSPC repo, the environment, the decay simulation, the tests>

**Speed comparison (loop vs NumPy):**

| version | time (s) |
|---------|----------|
| pure-Python loop | ... |
| NumPy (vectorised) | ... |

- Speed-up: **... × faster**

**Tests:** all passing? (yes / no)

**Conclusion:**
- <2–3 sentences: what worked, what you learned, any problems you hit and how you solved them>

---

<!-- Future sessions: add a new "## PW<n> — Lab <X>" section below. -->

## PW1 --- Lab B

**Data Observation:**
The dataset in `decay_observed.csv` shows an exponential decay of count values over time.

**Model Comparison:**
Upon visual analysis of the generated plot, the observed data points closely match the theoretical analytical curve ($N(t) = N_0 \cdot e^{-\lambda t}$), validating the exponential decay law.

**Snakemake Automation:**
The Snakemake pipeline automates the plot generation by running `plot.py` to create and update `figure.png` automatically whenever the input data or script changes.