# Adaptive Diffusion Security

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E)
![AI Security](https://img.shields.io/badge/Domain-AI%20Security-blue)
![Status](https://img.shields.io/badge/Status-Completed-green)

## Overview

An experimental study of adversarial robustness in text-to-image
generative AI systems, focusing on Stable Diffusion, adaptive
perturbation-length selection and semantic defence evaluation.

This project investigates how adversarial text perturbations affect
CLIP representations and the reliability of semantic detection
mechanisms.

Developed as part of the Master of Artificial Intelligence
programme at Monash University Malaysia, 2026.

## Research Objectives

- Reproduce the Query-Free Adversarial Attack framework.
- Investigate adaptive PGD perturbation-length selection.
- Evaluate robustness across different random seeds.
- Analyse semantic defence responses to perturbed prompts.
- Investigate false-positive vulnerabilities in AI defence systems.

## Technical Stack

| Technology | Application |
|---|---|
| Python | Experimental implementation |
| PyTorch | Deep learning and optimisation |
| Stable Diffusion v1.4 | Text-to-image generation |
| CLIP | Text representation analysis |
| BART-large-MNLI | Semantic intent classification |
| PGD | Adversarial optimisation |
| Hugging Face | Pretrained model integration |
| Google Colab | Experimental environment |

## Experimental Framework

The project consists of four principal components:

1. Query-free adversarial baseline reproduction.
2. Adaptive PGD perturbation-length evaluation.
3. Controlled Stable Diffusion image generation.
4. Semantic defence robustness analysis.

## Key Experimental Results

### Adaptive PGD Evaluation

The initial experiment reduced the perturbation length
from five to four, representing a 20% reduction while
preserving the predefined optimisation objective.

| Metric | Fixed PGD | Adaptive PGD |
|---|---:|---:|
| Perturbation length | 5 | 4 |
| PGD objective value | 1.9438 | 2.0139 |

### Robustness Across Random Seeds

| Seed | Fixed PGD Loss | Adaptive PGD Loss | Selected Length |
|---|---:|---:|---:|
| 27 | 1.9438 | 2.0139 | 4 |
| 42 | 1.7680 | 1.7306 | 2 |
| 100 | 1.9022 | 1.9692 | 4 |

All three evaluated seeds selected shorter perturbation
lengths while satisfying their respective experimental
effectiveness criteria.

### Semantic Defence Evaluation

The results demonstrated that adversarial optimisation
performance and semantic defence responses are not
necessarily aligned.

The evaluation also identified a false-positive
vulnerability in the tested semantic detection component,
highlighting the importance of assessing defence reliability.

## Individual Contributions

This portfolio focuses on my individual contributions
to the original collaborative academic project:

- Semantic defence evaluation and analysis.
- Adaptive false-positive robustness investigation.
- Interpretation of adversarial optimisation performance.
- Critical analysis of defence limitations.
- Evaluation of experimental methodology.

Relevant shared baseline implementation and collaborative
adaptive PGD experiments are retained with attribution.
Other team members' individual strategies are excluded.

## Key Findings

- Perturbation length and optimisation performance do
  not necessarily exhibit a monotonic relationship.
- Embedding-level optimisation does not independently
  establish generated image behaviour.
- Semantic defence reliability requires separate evaluation.
- Adversarial robustness is dependent on the evaluation
  objective and model configuration.

## Limitations

- Limited prompt diversity and random seed coverage.
- Small-scale visual evaluation.
- Findings are specific to the evaluated model and
  defence configurations.
- Quantitative image-level concept removal was not
  comprehensively validated.

## Responsible Research

This project was conducted in a controlled academic
environment using benign experimental prompts.

Its purpose is to understand adversarial machine learning,
evaluate generative AI security and identify limitations
in existing defence mechanisms.

## References

Zhuang, H., Zhang, Y., & Liu, S. (2023).
*A Pilot Study of Query-Free Adversarial Attack Against
Stable Diffusion*. IEEE/CVF Conference on Computer Vision
and Pattern Recognition Workshops (CVPRW).

Acknowledgement is extended to the original QF-Attack
research authors, the academic project collaborator,
and the Light.PixelGuard team for their defence framework.

## Author

**Lekshmy Natesh**

Master of Artificial Intelligence  
Monash University Malaysia

Research Interests: Deep Learning, Generative AI,
Adversarial Machine Learning and AI Security.
