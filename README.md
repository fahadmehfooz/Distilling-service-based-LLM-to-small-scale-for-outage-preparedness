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

├── Finetuneing_Teacher_Model.ipynb              # Fine-tuning Llama 7B using QLoRA and PEFT

├── Synthetic_Data_Generation_with_Scoring.ipynb # Generates synthetic datasets and scores them
├── Knowledge Distillation Llama to Gemma.ipynb  # Distillation from Llama 7B to Gemma 2B
├── README.md                                    # Project overview and instructions
└── requirements.txt                             # List of dependencies for the project

## Notebooks

1. **Finetuneing_Teacher_Model.ipynb**: Fine-tunes LLaMA 7B using QLoRA and PEFT.
2. **Synthetic_Data_Generation_with_Scoring.ipynb**: Generates and scores synthetic datasets.
3. **Knowledge Distillation Llama to Gemma.ipynb**: Performs knowledge distillation from LLaMA 7B to Gemma 2B.

## Datasets

Synthetic datasets are generated using Langchain and few-shot learning with Llama 405B. These datasets are scored for correctness using NVIDIA NeMoTron, achieving a 15% improvement in correctness scores.

Access the synthetic datasets via this [Google Drive link](insert_link_here).

## Installation

```bash
git clone https://github.com/your-username/distilling-llm-project.git
cd distilling-llm-project
pip install -r requirements.txt

Usage
Open and run the notebooks in the following order:
Synthetic_Data_Generation_with_Scoring.ipynb
Finetuneing_Teacher_Model.ipynb
Knowledge Distillation Llama to Gemma.ipynb
Follow the instructions within each notebook to execute the respective processes.
Results
Model Compression: 71% parameter reduction (LLaMA 7B to Gemma 2B)
Performance Improvement: 40% faster response time
Data Quality: 15% improvement in synthetic data correctness scores

Future Work
Further optimize the distillation process
Explore new methods for generating higher-quality synthetic datasets
Investigate applicability to other models and use cases
Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgements
Hugging Face for providing pre-trained models and libraries
NVIDIA for NeMoTron scoring improvements
LangChain for synthetic data generation tools
