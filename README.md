# Distilling Service-Based LLM to Small-Scale for Outage Preparedness

This project focuses on fine-tuning and knowledge distillation of large language models (LLMs) to smaller, more efficient models for preparedness in case of outages. The goal is to compress models like LLaMA 7B to Gemma 2B, reducing parameters by approximately 71% and improving response time by 40% while maintaining minimal accuracy loss.

## Key Features

- Fine-tuning of LLaMA 7B using QLoRA and PEFT techniques
- Synthetic dataset generation using Langchain and Llama 405B
- Dataset scoring improvements using NVIDIA NeMoTron
- Knowledge distillation from LLaMA 7B to Gemma 2B

## Project Structure

distilling-llm-project/
│

├── Finetuning_Teacher_Model.ipynb              # Fine-tuning Llama 7B using QLoRA and PEFT

├── Synthetic_Data_Generation_with_Scoring.ipynb # Generates synthetic datasets and scores them

├── Knowledge Distillation Llama to Gemma.ipynb  # Distillation from Llama 7B to Gemma 2B

├── README.md                                    # Project overview and instructions

└── requirements.txt                             # List of dependencies for the project

## Notebooks

1. **Finetuneing_Teacher_Model.ipynb**: Fine-tunes LLaMA 7B using QLoRA and PEFT.
2. **Synthetic_Data_Generation_with_Scoring.ipynb**: Generates and scores synthetic datasets.
3. **Knowledge Distillation Llama to Gemma.ipynb**: Performs knowledge distillation from LLaMA 7B to Gemma 2B.

## Datasets

- Synthetic datasets are generated using Langchain and few-shot learning with Llama 405B.
- These datasets are scored for correctness using NVIDIA NeMoTron, achieving a 15% improvement in correctness scores.

## Installation

Running the Notebooks
Fine-Tuning the Teacher Model:

Open the Finetuneing_Teacher_Model.ipynb notebook.
Execute the cells to fine-tune the Llama 7B model using QLoRA and PEFT on the synthetic datasets.
Generating Synthetic Data:

Open the Synthetic_Data_Generation_with_Scoring.ipynb notebook.
Run the cells to generate synthetic datasets using Langchain, and score the datasets with NVIDIA NeMoTron.

## Knowledge Distillation:

Open the Knowledge Distillation Llama to Gemma.ipynb notebook.
Execute the steps for distilling the Llama 7B model to Gemma 2B, and evaluate the smaller model’s performance.

## Results

Model Compression: LLaMA 7B was successfully compressed into Gemma 2B, achieving a 71% parameter reduction.
Performance Improvement: Response time improved by 40% with minimal loss in accuracy.
Data Generation: High-quality synthetic data was generated, improving correctness scores by 15% via NVIDIA NeMoTron.
