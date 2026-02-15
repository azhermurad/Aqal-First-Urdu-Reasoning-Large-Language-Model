# Urdu Reasoning LLM

## Aqal: The First Urdu Reasoning Large Language Model through Continued Pretraining and GRPO-Based Reinforcement Learning

------------------------------------------------------------------------

# 1. Project Overview

This project aims to develop and evaluate the first reasoning-optimized
Urdu Large Language Model (LLM). The project investigates whether
reasoning performance in Urdu can be significantly improved through a
structured three-stage training pipeline:

1.  Continued Pretraining (CPT)\
2.  Supervised Fine-Tuning (SFT)\
3.  GRPO-based Reinforcement Learning (RL)

The system focuses on improving multi-step reasoning, logical
consistency, and final-answer correctness in Urdu.

------------------------------------------------------------------------
<!-- 
# 2. Repository Structure

project/ │ ├── README.md\
├── requirements.txt\
├── environment.yml\
├── .env.example\
│ ├── src/\
│ ├── **init**.py\
│ ├── data/\
│ ├── models/\
│ ├── evaluation/\
│ ├── service/\
│ ├── utils/\
│ └── configs/\
│ └── default.yaml\
│ ├── scripts/\
│ ├── train.py\
│ ├── eval.py\
│ └── run_pipeline.py\
│ ├── tests/\
│ └── test\_\*.py\
│ ├── artifacts/\
│ ├── models/\
│ ├── logs/\
│ └── reports/\
│ ├── A1/\
│ ├── A1_Report.pdf\
│ └── latex_source.zip\
│ ├── A2/\
├── A3/\
└── A4/

------------------------------------------------------------------------

# 3. Environment Setup

## Using Conda (Recommended)

conda env create -f environment.yml\
conda activate urdu_reasoning_llm

## Using pip

pip install -r requirements.txt

Python 3.10+ recommended.

------------------------------------------------------------------------

# 4. Training Pipeline

## Continued Pretraining

python scripts/train.py --config src/configs/default.yaml --stage cpt

## Supervised Fine-Tuning

python scripts/train.py --config src/configs/default.yaml --stage sft

## GRPO Reinforcement Learning

python scripts/train.py --config src/configs/default.yaml --stage grpo

------------------------------------------------------------------------

# 5. Evaluation

python scripts/eval.py --checkpoint artifacts/models/grpo/ --dataset
src/data/eval_dataset.jsonl

Evaluation metrics include Final Answer Accuracy, Exact Match, Logical
Consistency, and Perplexity.

------------------------------------------------------------------------

# 6. Reproducibility

To reproduce complete results:

python scripts/run_pipeline.py --stage all --config
src/configs/default.yaml

All outputs are stored in artifacts/models, artifacts/logs, and
artifacts/reports.

------------------------------------------------------------------------

# 7. License

Academic use only -- CS818 Large Language Models.

------------------------------------------------------------------------

# 8. Contact

Azher Ali\
MS Data Science -- SEECS, NUST -->