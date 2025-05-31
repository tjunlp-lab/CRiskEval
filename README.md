# CRiskEval: A Chinese Multi-Level Risk Evaluation Benchmark Dataset for Large Language Models

<div align="center">
 <a href='https://arxiv.org/abs/2406.04752'><img src='https://img.shields.io/badge/Paper-arXiv-red'></a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
 <a href=''><img src='https://img.shields.io/badge/License-MIT-blue'></a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

 <br>
 <br>
</div>

![image](https://github.com/tjunlp-lab/CRiskEval/blob/main/Taxonomy.png)

*Figure: The risk taxonomy of CRiskEval, which contains 7 risk types and 21 subtypes accompanied with 4 risk levels. The proportion of each risk type is also presented here. The examples of each risk subtype are provided in [Examples.md](https://github.com/tjunlp-lab/CRiskEval/blob/main/RiskTaxonomy.png)*

## Overview

**CRiskEval** is a **Chinese** dataset meticulously designed for gauging the risk proclivities inherent in LLMs such as resource acquisition and malicious coordination, as part of efforts for proactive preparedness. To curate CRiskEval, we define a new risk taxonomy with **7 types of frontier risks** and **4 safety levels**, including extremely  hazardous,moderately hazardous, neutral and safe. We follow the philosophy of tendency evaluation to  empirically measure the stated ``desire'' of LLMs via fine-grained multiple-choice question answering. The dataset consists of 14,888 questions that simulate scenarios related to predefined 7 types of frontier risks. Each question is accompanied with 4 answer choices that state opinions or behavioral tendencies corresponding to the question. All answer choices are manually annotated with one of the defined risk levels so that we can easily build a fine-grained frontier risk profile for each assessed LLM.


## Data Curation

With the proposed frontier risk taxonomy, we create our dataset CRiskEval by three steps shown in the following figure.

![image](https://github.com/tjunlp-lab/CRiskEval/blob/main/DataCurationProcess.png)

*Figure: Diagram for data construction and model evaluation. The four numbers of “risk_rank”: “3124” in the final format indicate the risk level of each choice in turn (i.e., choice A is at the risk level of 3, choice B risk level 1, so on and so forth).*
 
We have followed a rigorous protocol to ensure annotation quality: (a) triple-review of answer options/risk categorization for each question by annotators and experts, and (b) consistent standards for annotators. The criteria for annatation is provided in [RiskLevelCriteria.md](https://github.com/tjunlp-lab/CRiskEval/blob/main/Risk%20level%20criteria.md)

---

> **Academic Citation**:  
> Our paper details the technical implementation.  
> ```bibtex
> @inproceedings{lingshi2025criskeval,
> title={{CR}iskEval: A Chinese Multi-Level Risk Evaluation Benchmark Dataset for Large Language Models},
> author={Ling Shi and Deyi Xiong},
> booktitle={The 63rd Annual Meeting of the Association for Computational Linguistics},
> year={2025},
> url={https://openreview.net/forum?id=ykenRgXIN0}
> }
> ```
