# ml-journey

Learning machine learning from the foundations up, in public. Every derivation, notebook and project from the plan lands here, with a short log entry each week.

**How I work:** two focused blocks a day (90 min + 60 min), Monday to Saturday. Sundays are rest days or a 25-minute checkpoint. Ideas and questions outside the current week go to [PARKING.md](PARKING.md) so they do not turn into detours.

## Plan: first 4 weeks (16 Nov to 13 Dec 2026)

| Week | Dates | Phase | Focus |
|---|---|---|---|
| 1 | 16 to 22 Nov | P0 Setup | Repo and machine, free GPUs (Kaggle, Colab), Anki deck, math gap check, linear regression by hand and in NumPy, Karpathy's training recipe |
| 2 | 23 to 29 Nov | P1 Foundations | Bias and variance, evaluation, regularization and learning curves, logistic regression, softmax derivation, neural network intuition |
| 3 | 30 Nov to 6 Dec | P1 Foundations | Backprop by hand, vectorized gradients and gradient check, PyTorch tensors, autograd and modules, a first training loop |
| 4 | 7 to 13 Dec | P1 Foundations | PyTorch training loop, overfit one batch, validation, optimizers, regularization in practice, Project 0, midpoint check |

## Weekly log

One row per week: what shipped, what slipped, what comes next.

| Week | Dates | Shipped | Slipped | Next |
|---|---|---|---|---|
| 1 | 16 to 22 Nov 2026 | **16 Nov:** created this repo, wrote this README and [PARKING.md](PARKING.md). Set up Python 3.12 with uv, installed PyTorch 2.15 and NumPy; the Apple GPU (MPS) works. | | A GPU run on Kaggle, the ML Core Anki deck |

## Setup

Python 3.12 in a virtual environment, managed with [uv](https://docs.astral.sh/uv/) (`brew install uv`):

```bash
uv venv --python 3.12
source .venv/bin/activate
uv pip install torch numpy
python -c 'import torch; print(torch.__version__)'
```
