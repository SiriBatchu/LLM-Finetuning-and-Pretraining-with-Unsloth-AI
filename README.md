# LLM-Finetuning-and-Pretraining-with-Unsloth-AI

# Project Overview

This repository contains code, Colab notebooks, and video tutorials demonstrating various techniques for fine-tuning, aligning, and deploying large language models (LLMs) using the Unsloth library for high-performance training.

The project covers the following key workflows (corresponding to assignment parts A-G):

A: Fine-tuning open-weight LLMs for specific tasks (e.g., coding instruction following with Llama 3.1).

Efficient Fine-tuning using QLoRA adapters with Unsloth optimizations.
Uses 4-bit quantization for significant memory reduction.
Demonstrated instruction following for coding tasks with Llama 3.1.

Colab : https://colab.research.google.com/drive/1n0b6kpqQadta9A8ORhJr7JEgdO05gY_b

B: Continued pretraining to adapt models to new languages (e.g., teaching TinyLlama Hindi).

Adapting LLMs to New Languages by continued pretraining on raw text corpora (e.g., Hindi).
Improves vocabulary and pattern recognition for the target language (demonstrated with TinyLlama).

Colab : https://colab.research.google.com/drive/15FAnxvHmE_1R9xXzmzoKHnpihtZVLEnI

C: Advanced Chat Template Applications including classification, conversational chat, extending TinyLlama's context window, and fine-tuning on multiple datasets simultaneously.

Utilizing chat templates for various tasks beyond simple conversation:
Framing Classification as an instruction task.
Handling multi-turn Conversational Chat.
Extending Max Context Size for models like TinyLlama using Unsloth's features.
Combining Multiple Datasets (e.g., chat and code) into a single fine-tuning run.

Colab : https://colab.research.google.com/drive/1BAjHqerVKCKSJTYh9wqK6UguhTVG_jst

D: Reward modeling using ORPO and DPO for preference alignment (using Phi-3 Mini).

Aligning model preferences using state-of-the-art techniques:
DPO (Direct Preference Optimization) using preference pairs.
ORPO (Odds Ratio Preference Optimization) combining LM loss with preference optimization.
Demonstrated with Phi-3 Mini on the Ultrafeedback dataset.

Colab : https://colab.research.google.com/drive/1-QmKcGToSHrGngXwd6RYFL3qZd07s3qI

E: Continued fine-tuning starting from previously saved custom LoRA checkpoints.

Loading previously saved LoRA adapter checkpoints.
Continuing the fine-tuning process, allowing for iterative improvement or adaptation.

Colab : https://colab.research.google.com/drive/11D6_y7nNWKo8Z7-9g9Q_teU9O2sdgaKK

F: Mental health chatbot development via fine-tuning Phi-3 Mini, with important ethical considerations.

Fine-tuning Phi-3 Mini on the Amod/mental_health_counseling_conversations dataset.
Focuses on generating empathetic and supportive responses.
Includes critical ethical considerations and disclaimers in the system prompt.

Colab : https://colab.research.google.com/drive/1r5zoJPu8Qc6u7Tt1g-PFcDsyfBKO9WGy

G: Model export to GGUF format for local inference with Ollama.

Merging fine-tuned LoRA adapters into the base model.
Exporting the merged model to GGUF format using Unsloth's save_pretrained_gguf.
Provides instructions for creating an Ollama Modelfile and running the model locally.

Colab : https://colab.research.google.com/drive/1MFptlFXvugWQuRuiYhjc5FsjEu_D0bAc

Youtube  : 

# Models Demonstrated

This project primarily demonstrates techniques using the following models fine-tuned with Unsloth:

Llama 3 / Llama 3.1 (8B): Used for instruction fine-tuning (Part A) and export to Ollama (Part G). Known for strong general language capabilities.

TinyLlama (1.1B): Used for continued pretraining (Part B), advanced chat template examples (Part C), and continued fine-tuning from checkpoints (Part E) due to its small size and speed.

Phi-3 Mini (3.8B): Used for reward modeling (DPO/ORPO, Part D) and the mental health chatbot (Part F) because of its balance between capability and efficiency.

Note: The techniques shown (fine-tuning, LoRA, DPO, ORPO, export) can often be applied to other compatible models listed in the Unsloth documentation with appropriate adjustments.

 
