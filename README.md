# abduction-syllogism-llm
_Evaluating Abductive Reasoning with Syllogistic Forms in Large Language Models_

Datasets and scripts for the HAR 2024 paper: ["Abductive Reasoning with Syllogistic Forms in Large Language Models"]()

## Contents

- [Contents](#contents)
- [Datasets](#datasets)
  - [Abduction Task Format](#abduction-task-format)
  - [Deduction Task Format](#deduction-task-format)
- [Citation](#citation)

## Datasets

### Abduction Task Format

#### File

[`data/Abduction_synthetic_problems.tsv`](https://github.com/kmineshima/abduction-syllogism-llm/blob/main/data/Abduction_synthetic_problems.tsv)

#### Description

| Column Name | Description |
| ---- | ---- |
| premises_en | two premises in English |
| hypothesis_en_1 | hypothesis 1 in English |
| hypothesis_en_2 | hypothesis 2 in English |
| gold | correct answer as abduction (1-3, 3 is *Neither is a good explanation.*) |
| gold_deduc | correct answer as deduction (1-3, 3 is *Neither is a good explanation.*) |
| figure_premises | the form of each premise (two letters composed of A, E, P and N) and code for the order in which each term appears (1-4) |
| content | classification based on belief consistency (*neutral*, *consistent*, *inconsistent*) |



- See [our paper](#citation) for details.

### Deduction Task Format

#### File

[`data/Deduction_synthetic_problems.tsv`](https://github.com/kmineshima/abduction-syllogism-llm/blob/main/data/Deduction_synthetic_problems.tsv)

#### Description

| Column Name | Description |
| ---- | ---- |
| premises_en | two premises in English |
| hypothesis_en_1 | hypothesis 1 in English |
| hypothesis_en_2 | hypothesis 2 in English |
| gold | correct answer as deduction (1-3, 3 is *Neither.*) |
| figure_premises | the form of each premise (two letters composed of A, E, P and N) and code for the order in which each term appears (1-4) |
| content | classification based on belief consistency (*neutral*, *consistent*, *inconsistent*) |

- See [our paper](#citation) for details.
<!-- - **NOTE:** One of the five hypotheses is "none of them". -->

## Citation

If you use this data in any published research, please cite the following:

- Hirohiko Abe, Risako Ando, Takanobu Morishita, Kentaro Ozeki, Koji Mineshima, and Mitsuhiro Okada, ["Abductive Reasoning with Syllogistic Forms in Large Language Models"](), *Proceedings of the 3rd International Conference on Human and Artificial Rationalities* (HAR 2024), Lecture Notes in Computer Science (LNAI), 2024.

<!-- ```
@InProceedings{ando-et-al-2024-euler-diagrams-llm,
author="Ando, Risako and Ozeki, Kentaro and Morishita, Takanobu and Abe, Hirohiko and Mineshima, Koji and Okada, Mitsuhiro",
editor="Lemanski, Jens and Johansen, Mikkel Willum and Manalo, Emmanuel
and Viana, Petrucio and Bhattacharjee, Reetu and Burns, Richard",
title="Can Euler Diagrams Improve Syllogistic Reasoning in Large Language Models?",
booktitle="Diagrammatic Representation and Inference",
series="Lecture Notes in Computer Science (LNAI)",
volume="14981",
year="2024",
publisher="Springer",
pages="232--248",
doi="https://doi.org/10.1007/978-3-031-71291-3_19"
}
``` -->
