# Personas with Attitudes
 
This repository contains the code used to implement experiments on injecting subjectivity into LLM-generated annotations via persona descriptions. For detailed information, refer to our paper:
 
> Fröhling, L., Demartini, G. & Assenmacher, D. (2024). *Personas with Attitudes: Controlling LLMs for Diverse Data Annotation*. arxiv identifier coming soon...
 
## Reproducing LLM Annotations
 
LLM annotations can be reproduced using the following Jupyter notebooks:
- `[model]_llm_1_2.ipynb`
- `[model]_llm_3_4.ipynb`
- `[model]_llm_4.ipynb`
 
### Available Models
The available model alternatives for `[model]` are:
- **Mistral**: [Mistral-7B-v0.1](https://huggingface.co/mistralai/Mistral-7B-v0.1)
- **Qwen**: [Qwen2-7B-Instruct](https://huggingface.co/Qwen/Qwen2-7B-Instruct)
 
These models need to be downloaded and deployed via the Llama CPP Python bindings, which can be found [here](https://github.com/abetlen/llama-cpp-python). The provided code assumes the existence of `.gguf` files that can be produced using the converter available from [Llama CPP](https://github.com/ggerganov/llama.cpp).
 
## Datasets
 
We exclusively rely on publicly available datasets for all experiments:
- **Persona Descriptions**: 200,000 persona descriptions from the [Persona Hub](https://github.com/tencent-ailab/persona-hub) (need to be parsed from `.jsonl` to `.pkl` format).
- **Toxicity Datasets**: Crowd-annotated toxicity datasets provided by [Sap et al.](https://maartensap.com/racial-bias-hatespeech/).
 
## Processing and Analysis
 
The processing and analysis steps are available in the remaining `.ipynb` files.
