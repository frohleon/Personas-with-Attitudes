# Personas-with-Attitudes
This repository contains the code that was used to implement experiments on the injection of subjectivity into LLM-generated annotations via persona descriptions. Detailed information can be found in our paper:

Fröhling, L., Demartini, G. & Assenmacher, D. (2024) Personas with Attitudes: Controlling LLMs for Diverse Data Annotation. arxiv...

LLM annotations can be reproduced via the [model]_llm_1_2.ipynb, [model]_llm_3_4.ipynb and [model]_llm_4.ipynb jupyter notebooks, where the available alternatives for [model] are mistral and qwen.
The mistral (https://huggingface.co/mistralai/Mistral-7B-v0.1) and qwen (https://huggingface.co/Qwen/Qwen2-7B-Instruct) model variants need to be downloaded and deployed via the llama cpp python bindings (https://github.com/abetlen/llama-cpp-python). The code provided here thus presupposes the existence of the corresponding .gguf files that can be produced via the converter available from llama cpp (https://github.com/ggerganov/llama.cpp).

For all experiments, we exclusively rely on publicly available datasets:
- the 200,000 available persona descriptions from the Persona Hub (https://github.com/tencent-ailab/persona-hub; need to be parsed from .jsonl to .pkl format) and
- the crowd-annotated toxicity datasets provided by Sap et al. (https://maartensap.com/racial-bias-hatespeech/)

Folders starting with [model]_llm contain the LLM annotations that are generated by runing the [model]_llm files. Folders starting with [model]_study are by design empty and will contain the intermediate data produced during the processing and analysis steps. Processing and analysis steps are available from the remaining .ipynb files.
