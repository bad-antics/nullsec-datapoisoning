<div align="center">

# ☠️ NullSec DataPoisoning

### Training Data Poisoning Detection & Simulation

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)]()
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)]()
[![NullSec](https://img.shields.io/badge/NullSec-Linux_v5.0-00ff41?style=for-the-badge&logo=linux&logoColor=white)](https://github.com/bad-antics/nullsec-linux)

*Detect, simulate, and defend against training data poisoning attacks*

</div>

---

## 🎯 Overview

NullSec DataPoisoning provides tools for detecting and simulating data poisoning attacks against machine learning pipelines. It implements backdoor injection (BadNets, Trojaning), clean-label attacks, and gradient-based poisoning, alongside detection methods like spectral signatures, activation clustering, and STRIP.

## ⚡ Features

| Feature | Description |
|---------|-------------|
| **Backdoor Injection** | BadNets, Trojan, blend, and warp triggers |
| **Clean-Label Attacks** | Feature collision, convex polytope, Witches' Brew |
| **Detection Engine** | Spectral signatures, activation clustering, STRIP |
| **Neural Cleanse** | Reverse-engineer trigger patterns from poisoned models |
| **Dataset Audit** | Scan datasets for anomalous samples and label flips |
| **Pipeline Scanner** | Audit ML pipelines for poisoning entry points |

## 📋 Attack & Defence Matrix

| Technique | Category | Type |
|-----------|----------|------|
| BadNets | Backdoor | Attack |
| Trojan Attack | Backdoor | Attack |
| Clean-Label FC | Poisoning | Attack |
| Witches' Brew | Poisoning | Attack |
| Spectral Signatures | Statistical | Defence |
| Activation Clustering | Neural | Defence |
| STRIP | Runtime | Defence |
| Neural Cleanse | Reverse Engineering | Defence |

## 🚀 Quick Start

```bash
# Scan a dataset for poisoning indicators
nullsec-datapoisoning scan --dataset training_data/ --model model.pt

# Simulate backdoor attack
nullsec-datapoisoning inject --dataset clean.csv --trigger patch --target-label 0 --poison-rate 0.01

# Run Neural Cleanse detection
nullsec-datapoisoning cleanse --model suspect_model.pt --num-classes 10

# Audit an ML pipeline config
nullsec-datapoisoning audit --pipeline pipeline.yaml
```

## 🔗 Related Projects

| Project | Description |
|---------|-------------|
| [nullsec-adversarial](https://github.com/bad-antics/nullsec-adversarial) | Adversarial ML attack toolkit |
| [nullsec-modelaudit](https://github.com/bad-antics/nullsec-modelaudit) | ML model security auditing |
| [nullsec-llmred](https://github.com/bad-antics/nullsec-llmred) | LLM red-teaming framework |
| [nullsec-promptinject](https://github.com/bad-antics/nullsec-promptinject) | Prompt injection payloads |
| [nullsec-linux](https://github.com/bad-antics/nullsec-linux) | Security Linux distro (140+ tools) |

## ⚠️ Legal

For **authorized ML security research only**. Poisoning production training data without authorization is illegal.

## 📜 License

MIT License — [@bad-antics](https://github.com/bad-antics)

---

<div align="center">

*Part of the [NullSec AI/ML Security Suite](https://github.com/bad-antics)*

</div>
