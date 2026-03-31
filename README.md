# Dynamic LLM Trainer Framework for Kubeflow

## Proposal Overview

This project enhances **Kubeflow Trainer** by creating a **dynamic, pluggable LLM training framework**. Currently, Kubeflow Trainer relies on **TorchTune**, which limits support for new models and advanced fine-tuning methods like **DPO, PPO, ORPO**.  

The goal is to **decouple the trainer from any single backend**, enabling multiple frameworks to integrate seamlessly while keeping **backward compatibility** and a **Python-first SDK**.

---

## Key Features

- **Pluggable Architecture:** Easily integrate multiple backends (TorchTune, TRL, Unsloth, LlamaFactory).  
- **Dynamic Backend Registration:** Supports in-tree and external frameworks.  
- **Python SDK Friendly:** Simple interface for distributed LLM training.  
- **Backward Compatibility:** Existing TorchTune workflows continue to work.  
- **Faster Model Support:** Day-0/Day-1 support for new models and fine-tuning strategies.

---


**Backend Flow:**
User → Python SDK → Kubeflow Trainer → Backend Modules


**Backends:**

- **TorchTune:** Maintains existing functionality  
- **TRL:** Industry standard for SFT/DPO/PPO workflows  
- **Unsloth:** ~2× faster, ~70% lower memory  
- **LlamaFactory:** 100+ model support  

---

## Skills Demonstrated

- Python & Go for ML systems  
- Distributed training concepts  
- API and framework design  
- Kubernetes & Kubeflow Trainer architecture  
- LLM fine-tuning knowledge (TRL, TorchTune, Unsloth)

---

## Why This Project

This project bridges **modern LLM tooling** with **production-ready Kubernetes platforms**, enabling developers and ML engineers to scale **large language model training** efficiently while staying flexible and modular.

---

## Repository Status

📌 **Proposal Stage** – This repository contains the **proposal documentation and visuals only**. Code implementation will follow if accepted into GSoC 2026.

---
