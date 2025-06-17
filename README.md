# LLMs for SWE-Bench: Solving Real-World GitHub Issues
A reading list on large language models solving real-world GitHub issues.

<div align="center">

[![LICENSE](https://img.shields.io/github/license/wasiahmad/Awesome-LLM-SWE-Bench)](https://github.com/wasiahmad/Awesome-LLM-SWE-Bench/blob/main/LICENSE)
![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)
[![commit](https://img.shields.io/github/last-commit/wasiahmad/Awesome-LLM-SWE-Bench?color=blue)](https://github.com/wasiahmad/Awesome-LLM-SWE-Bench/commits/main)
[![PR](https://img.shields.io/badge/PRs-Welcome-red)](https://github.com/wasiahmad/Awesome-LLM-SWE-Bench/pulls)
[![GitHub Repo stars](https://img.shields.io/github/stars/wasiahmad/Awesome-LLM-SWE-Bench)](https://github.com/wasiahmad/Awesome-LLM-SWE-Bench)
<!-- ![license](https://img.shields.io/bower/l/bootstrap?style=plastic) -->

</div>

This repo includes papers, tools, and blogs about LLMs for SWE-Bench.

Thanks for all the great contributors on GitHub!🔥⚡🔥

## Contents

- [1. Benchmarks](#1-benchmarks)
- [2. Pipeline-based Methods and Datasets](#2-pipeline-based-methods-and-datasets)
- [3. Agentic Methods and Datasets](#3-agentic-methods-and-datasets)
- [4. Subtopics](#4-subtopics)
  - [4.1. File Localization](#41-file-localization)
  - [4.2. Bug Fixing](#42-bug-fixing)
  - [4.3. Test Case Generation](#43-test-case-generation)
- [5. Blogs](#5-blogs)

## 1. Benchmarks

- **SWE-bench: Can Language Models Resolve Real-World GitHub Issues?**<br> 
  *Jimenez et al., 2024* [[Paper](https://arxiv.org/abs/2310.06770)][[GitHub](https://github.com/SWE-bench/SWE-bench/tree/main)][[Leaderboard](https://www.swebench.com/)][[Dataset](https://huggingface.co/datasets/princeton-nlp/SWE-bench)] <br>

- **SWE-bench Multimodal: Do AI Systems Generalize to Visual Software Domains?** <br>
  *Yang et al., 2024* [[Paper](https://arxiv.org/abs/2410.03859)][[GitHub](https://github.com/SWE-bench/SWE-bench/tree/main)][[Leaderboard](https://www.swebench.com/multimodal.html)]

- **SWE-bench Multilingual** <br>
  *Khandpur et al., 2024* [[Webpage](https://kabirk.com/multilingual)][[GitHub](https://github.com/SWE-bench/SWE-bench/tree/main)][[Dataset](https://huggingface.co/datasets/SWE-bench/SWE-bench_Multilingual)]

- **Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving** <br>
  *Zan et al., 2025* [[Paper](https://arxiv.org/pdf/2504.02605)][[GitHub](https://github.com/multi-swe-bench/multi-swe-bench)] [[Leaderboard](https://multi-swe-bench.github.io/)]

- **SWE-PolyBench: A Multi-language Benchmark for Repository Level Evaluation of Coding Agents** <br>
  *Rashid et al., 2025* [[Paper](https://arxiv.org/abs/2504.08703)][[GitHub](https://github.com/amazon-science/SWE-PolyBench)][[Leaderboard](https://amazon-science.github.io/SWE-PolyBench/)][[Dataset](https://huggingface.co/datasets/AmazonScience/SWE-PolyBench)]

- **SWE-bench Goes Live!** <br>
  *Zhang et al., 2025* [[Paper](https://arxiv.org/abs/2505.23419)][[GitHub](https://github.com/microsoft/SWE-bench-Live)][[Leaderboard](https://swe-bench-live.github.io/)][[Dataset](https://huggingface.co/datasets/SWE-bench-Live/SWE-bench-Live)]


## 2. Pipeline-based Methods and Datasets

- **Agentless: Demystifying LLM-based Software Engineering Agents** <br>
  *Xia et al., 2024* [[Paper](https://arxiv.org/abs/2407.01489)][[GitHub](https://github.com/OpenAutoCoder/Agentless)]

- **PatchPilot: A Cost-Efficient Software Engineering Agent with Early Attempts on Formal Verification** <br>
  *Li et al., 2025* [[Paper](https://arxiv.org/abs/2502.02747)][[GitHub](https://github.com/ucsb-mlsec/PatchPilot)]

- **SWE-Fixer: Training Open-Source LLMs for Effective and Efficient GitHub Issue Resolution** <br>
  *Xie et al., 2025* [[Paper](https://arxiv.org/abs/2501.05040)][[GitHub](https://github.com/InternLM/SWE-Fixer)]

- **SoRFT: Issue Resolving with Subtask-oriented Reinforced Fine-Tuning** <br>
  *Ma et al., 2025* [[Paper](https://arxiv.org/abs/2502.20127)]


## 3. Agentic Methods and Datasets

- **SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering** <br>
  *Yang et al., 2024* [[Paper](https://arxiv.org/abs/2405.15793)][[GitHub](https://github.com/SWE-agent/SWE-agent)]

- **OpenHands: An Open Platform for AI Software Developers as Generalist Agents** <br>
  *Wang et al., 2024* [[Paper](https://arxiv.org/abs/2407.16741)][[GitHub](https://github.com/All-Hands-AI/OpenHands)]

- **Training Software Engineering Agents and Verifiers with SWE-Gym** <br>
  *Pan et al., 2024* [[Paper](https://arxiv.org/pdf/2412.21139)][[GitHub](https://github.com/SWE-Gym/SWE-Gym)][[Data & Models](https://huggingface.co/SWE-Gym)]

- **SWE-smith: Scaling Data for Software Engineering Agents** <br>
  *Yang et al., 2025* [[Paper](https://arxiv.org/abs/2504.21798)][[GitHub](https://github.com/SWE-bench/SWE-smith)][[Webpage](https://swesmith.com/)]


## 4. Subtopics

### 4.1. File Localization

- **SweRank: Software Issue Localization with Code Ranking** <br>
  *Reddy et al., 2025* [[Paper](https://arxiv.org/abs/2505.07849)]

- **CoRet: Improved Retriever for Code Editing** <br>
  *Fehr et al., 2025* [[Paper](https://arxiv.org/abs/2505.24715)]

- **CoSIL: Software Issue Localization via LLM-Driven Code Repository Graph Searching** <br>
  *Jiang et al., 2025* [[Paper](https://arxiv.org/abs/2503.22424)][[GitHub](https://github.com/ZhonghaoJiang/CoSIL)]


### 4.2. Bug Fixing

- **SWE-Synth: Synthesizing Verifiable Bug-Fix Data to Enable Large Language Models in Resolving Real-World Bugs** <br>
  *Pham et al., 2025* [[Paper](https://arxiv.org/abs/2504.14757)][[GitHub](https://github.com/FSoft-AI4Code/SWE-Synth)][[Dataset](https://huggingface.co/swesynth)]


### 4.3. Test Case Generation

- **UTBoost: Rigorous Evaluation of Coding Agents on SWE-Bench** <br>
  *Yu et al., 2025* [[Paper](https://arxiv.org/abs/2506.09289)][[GitHub](https://github.com/CUHK-Shenzhen-SE/UTBoost)]


## 5. Blogs

- **Raising the bar on SWE-bench Verified with Claude 3.5 Sonnet** <br>
  *Engineering at Anthropic, 2025* [[Webpage](https://www.anthropic.com/engineering/swe-bench-sonnet)]


