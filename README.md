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

- [1. The Benchmark Suite (Evaluation & Data)](#1-the-benchmark-suite-evaluation--data)
    - [1.1 Foundation & Vision](#11-foundation--vision)
    - [1.2 Multilingual Benchmark Suites](#12-multilingual-benchmark-suites)
    - [1.3 High-Fidelity & "Anti-Memorization" Suites](#13-high-fidelity--anti-memorization-suites)
    - [1.4 Specialized Verticals](#14-specialized-verticals)
    - [1.5 Holistic & Agent-Centric Frameworks](#15-holistic--agent-centric-frameworks)
- [2. Methodology: From Pipelines to Agents](#2-methodology-from-pipelines-to-agents)
    - [2.1 Design Paradigms: Agentless vs. Agentic](#21-design-paradigms-agentless-vs-agentic)
    - [2.2 Learning & Optimization Strategies](#22-learning--optimization-strategies)
    - [2.3 Scaling Laws for Software Engineering](#23-scaling-laws-for-software-engineering)
- [3. Specialized Task Modules (The "Sub-components")](#3-specialized-task-modules-the-sub-components)
    - [3.1 Fault Localization & Graph-Based Retrieval](#31-fault-localization--graph-based-retrieval)
    - [3.2 Cognitive & Memory-Enhanced Localization](#32-cognitive--memory-enhanced-localization)
    - [3.3 Synthesis, Bug Fixing & Validation](#33-synthesis-bug-fixing--validation)
- [4. Blogs](#4-blogs)

## 1. The Benchmark Suite (Evaluation & Data)

### 1.1 Foundation & Vision

- **SWE-bench: Can Language Models Resolve Real-World GitHub Issues?** <br> 
  *Jimenez et al., 2024* [[Paper](https://arxiv.org/abs/2310.06770)][[GitHub](https://github.com/SWE-bench/SWE-bench/tree/main)][[Leaderboard](https://www.swebench.com/)][[Dataset](https://huggingface.co/datasets/princeton-nlp/SWE-bench)] <br>

- **SWE-bench Multimodal: Do AI Systems Generalize to Visual Software Domains?** <br>
  *Yang et al., 2024* [[Paper](https://arxiv.org/abs/2410.03859)][[GitHub](https://github.com/SWE-bench/SWE-bench/tree/main)][[Leaderboard](https://www.swebench.com/multimodal.html)]

- **SWE-Bench Mobile: Can Large Language Model Agents Develop Industry-Level Mobile Applications?** <br>
  *Tian et al., 2026* [[Paper](https://arxiv.org/abs/2602.09540)][[GitHub](?)][[Leaderboard](?)]


### 1.2 Multilingual Benchmark Suites

- **SWE-bench Multilingual** <br>
  *Khandpur et al., 2024* [[Webpage](https://kabirk.com/multilingual)][[GitHub](https://github.com/SWE-bench/SWE-bench/tree/main)][[Dataset](https://huggingface.co/datasets/SWE-bench/SWE-bench_Multilingual)]

- **Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving** <br>
  *Zan et al., 2025* [[Paper](https://arxiv.org/pdf/2504.02605)][[GitHub](https://github.com/multi-swe-bench/multi-swe-bench)] [[Leaderboard](https://multi-swe-bench.github.io/)]

- **SWE-PolyBench: A Multi-language Benchmark for Repository Level Evaluation of Coding Agents** <br>
  *Rashid et al., 2025* [[Paper](https://arxiv.org/abs/2504.08703)][[GitHub](https://github.com/amazon-science/SWE-PolyBench)][[Leaderboard](https://amazon-science.github.io/SWE-PolyBench/)][[Dataset](https://huggingface.co/datasets/AmazonScience/SWE-PolyBench)]
  
- **SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks?** <br>
  *Deng et al., 2025* [[Paper](https://arxiv.org/abs/2509.16941)][[GitHub](https://github.com/scaleapi/SWE-bench_Pro-os)][[Leaderboard](https://scale.com/leaderboard/swe_bench_pro_public)][[Dataset](https://huggingface.co/datasets/ScaleAI/SWE-bench_Pro)]


### 1.3 High-Fidelity & "Anti-Memorization" Suites

- **SWE-rebench: An Automated Pipeline for Task Collection and Decontaminated Evaluation of Software Engineering Agents**<br> 
  *Badertdinov et al., 2025* [[Paper](https://arxiv.org/abs/2505.20411)][[GitHub](https://github.com/SWE-rebench/SWE-bench-fork)][[Leaderboard](https://swe-rebench.com/)][[Dataset](https://huggingface.co/datasets/nebius/SWE-rebench-leaderboard)] <br>

- **SWE-bench Goes Live!** <br>
  *Zhang et al., 2025* [[Paper](https://arxiv.org/abs/2505.23419)][[GitHub](https://github.com/microsoft/SWE-bench-Live)][[Leaderboard](https://swe-bench-live.github.io/)][[Dataset](https://huggingface.co/datasets/SWE-bench-Live/SWE-bench-Live)]

- **SWE-Lancer: Can Frontier LLMs Earn $1 Million from Real-World Freelance Software Engineering?** <br> 
  *Miserendino et al., 2025* [[Paper](https://arxiv.org/abs/2502.12115)][[GitHub](https://github.com/openai/frontier-evals/tree/main/project/swelancer)][[Leaderboard](https://llm-stats.com/benchmarks/swe-lancer)] <br>


### 1.4 Specialized Verticals

- **SWT-Bench: Testing and Validating Real-World Bug-Fixes with Code Agents** <br>
  *Mündler et al., 2024* [[Paper](https://arxiv.org/abs/2406.12952)][[GitHub](https://github.com/logic-star-ai/swt-bench)][[Leaderboard](https://swtbench.com/)][[Dataset](https://huggingface.co/collections/eth-sri/swt-bench)]

- **SWE-Perf: Can Language Models Optimize Code Performance on Real-World Repositories?** <br>
  *He et al., 2025* [[Paper](https://arxiv.org/abs/2507.12415)][[GitHub](https://github.com/swe-perf/swe-perf)][[Leaderboard](https://swe-perf.github.io/leaderboard.html)][[Dataset](https://huggingface.co/datasets/SWE-Perf/SWE-Perf)]

- **OmniCode: A Benchmark for Evaluating Software Engineering Agents** <br>
  *Sonwane et al., 2026* [[Paper](https://arxiv.org/abs/2602.02262)][[GitHub](https://github.com/seal-research/OmniCode)][[Dataset](https://huggingface.co/datasets/seal-research/OmniCode/tree/main)]


### 1.5 Holistic & Agent-Centric Frameworks

- **SWE-Compass: Towards Unified Evaluation of Agentic Coding Abilities for Large Language Models** <br>
  *Xu et al., 2025* [[Paper](https://arxiv.org/abs/2511.05459)]


## 2. Methodology: From Pipelines to Agents

### 2.1 Design Paradigms: Agentless vs. Agentic

#### Static/Pipeline-based (Agentless)

- **Agentless: Demystifying LLM-based Software Engineering Agents** <br>
  *Xia et al., 2024* [[Paper](https://arxiv.org/abs/2407.01489)][[GitHub](https://github.com/OpenAutoCoder/Agentless)]

- **PatchPilot: A Cost-Efficient Software Engineering Agent with Early Attempts on Formal Verification** <br>
  *Li et al., 2025* [[Paper](https://arxiv.org/abs/2502.02747)][[GitHub](https://github.com/ucsb-mlsec/PatchPilot)]

#### Agentic & Interactive

- **SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering** <br>
  *Yang et al., 2024* [[Paper](https://arxiv.org/abs/2405.15793)][[GitHub](https://github.com/SWE-agent/SWE-agent)]

- **OpenHands: An Open Platform for AI Software Developers as Generalist Agents** <br>
  *Wang et al., 2024* [[Paper](https://arxiv.org/abs/2407.16741)][[GitHub](https://github.com/All-Hands-AI/OpenHands)]


### 2.2 Learning & Optimization Strategies

#### Supervised & Subtask Fine-Tuning

- **SWE-Fixer: Training Open-Source LLMs for Effective and Efficient GitHub Issue Resolution** <br>
  *Xie et al., 2025* [[Paper](https://arxiv.org/abs/2501.05040)][[GitHub](https://github.com/InternLM/SWE-Fixer)]

- **SoRFT: Issue Resolving with Subtask-oriented Reinforced Fine-Tuning** <br>
  *Ma et al., 2025* [[Paper](https://arxiv.org/abs/2502.20127)]

- **SWE-Lego: Pushing the Limits of Supervised Fine-tuning for Software Issue Resolving** <br>
  *Tao et al., 2026* [[Paper](https://arxiv.org/abs/2601.01426)]

#### Alignment & Verification

- **Training Software Engineering Agents and Verifiers with SWE-Gym** <br>
  *Pan et al., 2024* [[Paper](https://arxiv.org/pdf/2412.21139)][[GitHub](https://github.com/SWE-Gym/SWE-Gym)][[Data & Models](https://huggingface.co/SWE-Gym)]

- **R2E-Gym: Procedural Environments and Hybrid Verifiers for Scaling Open-Weights SWE Agents** <br>
  *Jain et al., 2024* [[Paper](https://arxiv.org/abs/2504.07164)][[GitHub](https://github.com/R2E-Gym/R2E-Gym)][[Data & Models](https://huggingface.co/R2E-Gym)]

- **SWE-Manager: Selecting and Synthesizing Golden Proposals Before Coding** <br>
  *Tan et al., 2026* [[Paper](https://arxiv.org/abs/2601.22956)]

- **SWE-RM: Execution-free Feedback For Software Engineering Agents** <br>
  *Shum et al., 2025* [[Paper](https://arxiv.org/abs/2512.21919)]

- **Agentic Rubrics as Contextual Verifiers for SWE Agents** <br>
  *Raghavendra et al., 2026* [[Paper](https://arxiv.org/abs/2601.04171)]


### 2.3 Scaling Laws for Software Engineering

#### Data Synthesis & Environment Scaling

- **SWE-smith: Scaling Data for Software Engineering Agents** <br>
  *Yang et al., 2025* [[Paper](https://arxiv.org/abs/2504.21798)][[GitHub](https://github.com/SWE-bench/SWE-smith)][[Webpage](https://swesmith.com/)]

- **Skywork-SWE: Unveiling Data Scaling Laws for Software Engineering in LLMs** <br>
  *Zeng et al., 2025* [[Paper](https://arxiv.org/abs/2506.19290)]
  
- **SWE-Mirror: Scaling Issue-Resolving Datasets by Mirroring Issues Across Repositories** <br>
  *Wang et al., 2025* [[Paper](https://arxiv.org/abs/2509.08724)]

- **SWE-Universe: Scale Real-World Verifiable Environments to Millions** <br>
  *Chen et al., 2026* [[Paper](https://arxiv.org/abs/2602.02361)]

- **SWE-Factory: An Automatic Issue Resolution Dataset Construction Pipeline via LLM-based Multi Agents** <br>
  *Guo et al., 2025* [[Paper](https://arxiv.org/abs/2506.10954)]

#### Inference & Training Scaling

- **SWE-Dev: Building Software Engineering Agents with Training and Inference Scaling** <br>
  *Wang et al., 2025* [[Paper](https://arxiv.org/abs/2506.07636)][[GitHub](https://github.com/THUDM/SWE-Dev)]
  
- **Nemotron-CORTEXA: Enhancing LLM Agents for Software Engineering Tasks via Improved Localization and Solution Diversity** <br>
  *Sohrabizadeh et al., 2025* [[Paper](https://openreview.net/pdf?id=k6p8UKRdH7)]

  
## 3. Specialized Task Modules (The "Sub-components")

### 3.1. Fault Localization & Graph-Based Retrieval

- **SweRank: Software Issue Localization with Code Ranking** <br>
  *Reddy et al., 2025* [[Paper](https://arxiv.org/abs/2505.07849)]

- **CoRet: Improved Retriever for Code Editing** <br>
  *Fehr et al., 2025* [[Paper](https://arxiv.org/abs/2505.24715)]

- **CoSIL: Software Issue Localization via LLM-Driven Code Repository Graph Searching** <br>
  *Jiang et al., 2025* [[Paper](https://arxiv.org/abs/2503.22424)][[GitHub](https://github.com/ZhonghaoJiang/CoSIL)]

- **LocAgent: Graph-Guided LLM Agents for Code Localization** <br>
  *Chen et al., 2025* [[Paper](https://arxiv.org/abs/2503.09089)][[GitHub](https://github.com/gersteinlab/LocAgent)]

- **Reformulate, Retrieve, Localize: Agents for Repository-Level Bug Localization** <br>
  *Caumartin et al., 2025* [[Paper](https://arxiv.org/abs/2512.07022)]


### 3.2 Cognitive & Memory-Enhanced Localization

- **The SWE-Bench Illusion: When State-of-the-Art LLMs Remember Instead of Reason** <br>
  *Liang et al., 2025* [[Paper](https://arxiv.org/abs/2506.12286)]

- **Extracting Conceptual Knowledge to Locate Software Issues** <br>
  *Wang et al., 2025* [[Paper](https://arxiv.org/abs/2509.21427)]
  
- **Improving Code Localization with Repository Memory** <br>
  *Wang et al., 2025* [[Paper](https://arxiv.org/abs/2510.01003)]


### 3.3 Synthesis, Bug Fixing & Validation

- **SWE-Synth: Synthesizing Verifiable Bug-Fix Data to Enable Large Language Models in Resolving Real-World Bugs** <br>
  *Pham et al., 2025* [[Paper](https://arxiv.org/abs/2504.14757)][[GitHub](https://github.com/FSoft-AI4Code/SWE-Synth)][[Dataset](https://huggingface.co/swesynth)]

- **UTBoost: Rigorous Evaluation of Coding Agents on SWE-Bench** <br>
  *Yu et al., 2025* [[Paper](https://arxiv.org/abs/2506.09289)][[GitHub](https://github.com/CUHK-Shenzhen-SE/UTBoost)]

## 4. Blogs

- **Raising the bar on SWE-bench Verified with Claude 3.5 Sonnet** <br>
  *Engineering at Anthropic, 2025* [[Webpage](https://www.anthropic.com/engineering/swe-bench-sonnet)]

- **Why SWE-bench Verified no longer measures frontier coding capabilities** <br>
  *OpenAI, 2026* [[Webpage](https://openai.com/index/why-we-no-longer-evaluate-swe-bench-verified/)]


<p align="right" style="font-size: 14px; color: #555; margin-top: 20px;">
    <a href="#readme-top" style="text-decoration: none; color: #007bff; font-weight: bold;">
        ↑ Back to Top ↑
    </a>
</p>

## Contributing

- Add a new paper or update an existing paper, thinking about which category the work should belong to.
- Use the same format as existing entries to describe the work.
- Add the abstract link of the paper (`/abs/` format if it is an arXiv publication).

**Don't worry if you do something wrong, it will be fixed for you!**

### Contributors

<a href="https://github.com/wasiahmad/Awesome-LLM-SWE-Bench/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=wasiahmad/Awesome-LLM-SWE-Bench" />
</a>

### Star History

[![Star History Chart](https://api.star-history.com/svg?repos=atfortes/Awesome-LLM-SWE-Bench&type=Timeline)](https://star-history.com/#atfortes/Awesome-LLM-SWE-Bench&Timeline)


