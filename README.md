# THE LINE — LLM Engineering Labs

## Project overview

This repository contains a practical training project for **هندسة تطبيقات النماذج اللغوية الكبيرة**. The lab exercises use **THE LINE** as an educational project scenario and apply LLM application-engineering concepts to sustainability topics such as energy efficiency, water management, sustainable materials, and smart infrastructure.

The project is a training prototype. It is **not an official NEOM or THE LINE system**, it does not connect to live project infrastructure, and it does not use real operational data.

The theme was selected to keep the labs connected to a Saudi engineering context. Saudi Vision 2030 identifies NEOM among its major projects, while the official THE LINE material highlights sustainability and innovation as core principles.

Official background:
- Saudi Vision 2030: https://www.vision2030.gov.sa/
- THE LINE: https://www.neom.com/en-us/regions/theline

## Author

**Awadh Mohammed Alhajri**  
## Training program

**Program:** هندسة تطبيقات النماذج اللغوية الكبيرة  
**Training materials:** أ. لطيفة سعد  
**SDAIA Academy GitHub:** https://github.com/SDAIAAcademy

## Repository contents

```text
the-line-llm/
├── README.md
├── requirements.txt
├── CHANGELOG.md
├── .gitignore
├── docs/
│   ├── TECHNICAL_DOCUMENTATION.md
│   └── context_budget.md
└── notebooks/
    ├── Lab_1_THE_LINE.ipynb
    ├── Lab_2_THE_LINE.ipynb
    ├── Lab_3a_THE_LINE.ipynb
    ├── Lab_3b_THE_LINE.ipynb
    ├── Lab_4_THE_LINE.ipynb
    ├── Lab_5_THE_LINE.ipynb
    └── Lab_6_THE_LINE.ipynb
```

## Lab progression

| Lab | Main concept | Project use |
|---|---|---|
| Lab 1 | LLM interface, conversation state, context window | Basic THE LINE engineering assistant skeleton |
| Lab 2 | Provider abstraction, routing, streaming, retry/fallback | Same request flow across simulated providers |
| Lab 3a | Structured extraction and validation | Engineering request extraction and validation |
| Lab 3b | Tool registry, authorization, bounded tool loop | Status checks and engineering consultation booking |
| Lab 4 | Guarded pipeline | Input checks, PII masking, output checks, attack tests |
| Lab 5 | Evaluation harness | Golden-set evaluation and regression gate |
| Lab 6 | Cost/latency optimisation setup | Replay, simple routing, token/cost/latency baseline |

## How to run

The notebooks are designed for **Google Colab** and should be run in order.

1. Open https://colab.research.google.com/.
2. Upload a notebook from the `notebooks/` folder.
3. Select **Runtime → Run all**.
4. Run the labs in this order: Lab 1, Lab 2, Lab 3a, Lab 3b, Lab 4, Lab 5, Lab 6.

The exercises use simulated clients and demo responses, so no external model API key is required. Lab 3a uses Pydantic v2.

For a local Python environment:

```bash
python -m pip install -r requirements.txt
```

## Technical notes

The implementation intentionally keeps the structure of the training labs while changing the original service scenario to the THE LINE sustainability-engineering scenario. The notebooks demonstrate patterns rather than production integrations. Values used for demo costs, latency, test targets, IDs, and secret codes are training values only.

For the detailed flow and design decisions, see [`docs/TECHNICAL_DOCUMENTATION.md`](docs/TECHNICAL_DOCUMENTATION.md).

## Version control

The repository uses Git with small, topic-based commits. Generated cache files, local environments, and notebook checkpoints are excluded through `.gitignore`. Future changes should be committed with short messages that describe the change clearly.
