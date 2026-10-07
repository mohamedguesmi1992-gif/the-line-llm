# THE LINE — LLM Engineering Labs

## Project Overview

This repository contains a practical training project developed for the course **هندسة تطبيقات النماذج اللغوية الكبيرة**.

The project uses **THE LINE** as an educational engineering scenario and applies the lab concepts to sustainability-related topics such as energy efficiency, water management, sustainable materials, and smart infrastructure.

This is a training prototype only. It is not an official NEOM or THE LINE system and does not use real operational project data.

## Author

**Awadh Mohammed Alhajri**

## Training Program

**Program:** هندسة تطبيقات النماذج اللغوية الكبيرة

**Training Materials:** أ. لطيفة سعد

**SDAIA Academy GitHub:** https://github.com/SDAIAAcademy

## Project Files

- Lab_1_THE_LINE.ipynb
- Lab_2_THE_LINE.ipynb
- Lab_3a_THE_LINE.ipynb
- Lab_3b_THE_LINE.ipynb
- Lab_4_THE_LINE.ipynb
- Lab_5_THE_LINE.ipynb
- Lab_6_THE_LINE.ipynb
- TECHNICAL_DOCUMENTATION.md
- context_budget.md
- CHANGELOG.md
- requirements.txt
- .gitignore

## Lab Progression

**Lab 1:** LLM interface, conversation state, and context window.

**Lab 2:** Provider abstraction, routing, streaming, retry, and fallback.

**Lab 3a:** Structured extraction and validation of engineering requests.

**Lab 3b:** Tool registry, authorization, bounded tool loop, and engineering consultation booking.

**Lab 4:** Guarded pipeline with input checks, PII masking, output checks, and attack testing.

**Lab 5:** Evaluation harness using a golden set and regression gate.

**Lab 6:** Cost and latency optimisation using replay, routing, and model selection.

## How to Run

The notebooks are designed for **Google Colab**.

1. Open https://colab.research.google.com/
2. Upload one of the lab notebooks from this repository.
3. Select **Runtime → Run all**.
4. Run the labs in this order:

Lab 1 → Lab 2 → Lab 3a → Lab 3b → Lab 4 → Lab 5 → Lab 6

The exercises use simulated clients and demonstration responses. No external model API key is required for the provided lab activities.

## Technical Documentation

For additional technical details, see:

[TECHNICAL_DOCUMENTATION.md](TECHNICAL_DOCUMENTATION.md)

## Version Control

This project uses Git for version control. Changes are recorded through clear commits, and unnecessary local files are excluded using `.gitignore`.
