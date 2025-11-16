# Session 9 and 10 -  Mediation Fallacy Inference and Causality

This repository contains the materials for **Week 5** of *Inference and Causality*.  
- Slides: see [`slides/`](./slides/) folder  
- Notebooks: see [`notebooks/`](./notebooks/) folder 

---
## Session Outline
This week focuses on common **causal fallacies** that arise when we condition on the wrong variables or fail to account for causal structure. Understanding these fallacies is essential for proper causal inference and avoiding misleading conclusions.

### Topics Covered

**1. Mediation Fallacy**
- Understanding the difference between total effects and direct effects
- Why adjusting for mediators blocks causal pathways
- Practical example: Education → Income → Health
- When to control for mediators (and when not to)

**2. Collider Bias and Survivorship Bias**
- How conditioning on a collider creates spurious correlations
- The danger of analyzing only selected samples (survivors, successful cases)
- Real-world example: Success stories and risk-taking
- Why we shouldn't draw causal conclusions from "winner" datasets

**3. Simpson's Paradox**
- Reversal of associations when aggregating vs. stratifying by confounders
- Classic kidney stone treatment example
- The importance of adjusting for confounding variables

**4. Berkson's Paradox**
- Spurious negative correlations induced by selection bias
- Hospital admission example: conditioning on hospitalization
- Understanding why independent causes appear correlated in selected samples


---
## 🚀 Environment Setup

Before starting, please **fork this repository** and create a fresh Python virtual environment.  
All required libraries are listed in `requirements.txt`.

> ⚠️ If you encounter errors during `pip install`, try removing the version pinning for the failing package(s) in `requirements.txt`.  
> On Apple M1/M2 systems you may also need to install additional system packages (the “M1 shizzle”).

---

### macOS / Linux (bash/zsh)

```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (PowerShell)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\Activate.ps1

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### Windows (Git Bash)
```bash
# Select Python version (if using pyenv)
pyenv local 3.11.3

# Create and activate virtual environment
python -m venv .venv
source .venv/Scripts/activate

# Upgrade pip and install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
```

You’re now ready to run the session notebooks!

Deactivate the environment when you’re done:
```bash
deactivate
```
