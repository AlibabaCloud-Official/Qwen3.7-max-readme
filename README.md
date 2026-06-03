# Qwen3.7: The Agent Frontier

Qwen3.7-Max is built to be a versatile agent foundation — equally capable of writing and debugging code, automating office workflows, and sustaining autonomous execution across hundreds or thousands of steps.

What sets Qwen3.7-Max apart is the breadth and depth of its agent capabilities. It excels as a coding agent, from frontend prototyping to complex multi-file engineering. It serves as a reliable office and productivity assistant through MCP integrations and multi-agent orchestration. It sustains coherent reasoning across extremely long horizons — as demonstrated by a 35-hour, fully autonomous kernel optimization run comprising over 1,000 tool calls. It generalizes across agent scaffolds, performing consistently whether deployed through Claude Code, OpenClaw, Qwen Code, or other frameworks.

- **Qwen3.7-Max** — now available via [Alibaba Cloud Model Studio](https://modelstudio.console.alibabacloud.com):
    - frontier coding agent: from frontend prototyping to complex software engineering
    - office productivity and workflow automation via MCP and multi-agent orchestration
    - sustained autonomous execution across long-horizon tasks
    - cross-scaffold generalization across diverse agent frameworks
- Call via API on [Alibaba Cloud Model Studio](https://modelstudio.console.alibabacloud.com).

## 📊 Benchmark Performance


| Benchmark | Opus-4.6 Max | K2.6 Thinking | GLM-5.1 Thinking | DS-V4-Pro Max | Qwen3.6-Plus | Qwen3.7-Max |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Coding Agent** | | | | | | |
| Terminal Bench 2.0-Terminus | 65.4 | 66.7 | 63.5 | 67.9 | 61.6 | **69.7** |
| SWE-Verified | 80.8 | 80.2 | -- | 80.6 | 78.8 | 80.4 |
| SWE-Pro | 57.3 | 59.5 | 58.8 | 59.0 | 56.6 | **60.6** |
| SWE-Multilingual | 77.5 | 76.7 | -- | 76.2 | 73.8 | **78.3** |
| NL2repo | **47.6** | 42.8 | 41.0 | 35.5 | 34.4 | 47.2 |
| SciCode | 51.9 | 52.2 | 45.1 | -- | 41.4 | **53.5** |
| QwenWebDev | **1617** | -- | 1564 | 1570 | 1500 | 1568 |
| QwenSVG | 1541 | 1325 | 1605 | 1506 | 1432 | **1608** |
| **General Agent** | | | | | | |
| Qwencllaw | **65.5** | 54.7 | 58.7 | 59.2 | 57.2 | 64.3 |
| CoWorkBench | **68.2** | 58.2 | 66.0 | 66.3 | 64.5 | 67.2 |
| ClawEval | **70.4** | 61.5 | 62.7 | 58.4 | 57.1 | 65.2 |
| SkillsBench | -- | 56.2 | 53.1 | 52.3 | 45.7 | **59.2** |
| BFCL-v4 | **76.7** | 71.3 | 70.9 | 70.6 | 68.9 | 75.0 |
| MCP-Mark | 56.7 | 55.9 | 57.5 | 57.1 | 48.2 | **60.8** |
| MCP-Atlas | 75.8 | 66.6 | 71.8 | 73.6 | 74.1 | **76.4** |
| Vitabench | -- | 39.1 | 45.1 | **51.9** | 42.8 | 47.9 |
| SpreadSheetBench-v1 | **89.3** | 84.5 | 85.2 | 84.9 | 80.2 | 87.0 |
| Kernel Bench L3 | **2.63/98%** | 1.41/80% | 2.00/78% | 1.07/54% | 1.03/48% | 1.98/96% |
| HLE w/ tools | 53.0 | **54.0** | 52.3 | 48.2 | 50.2 | 53.5 |
| QwenWorldBench | 56.1 | 50.9 | 50.2 | 52.3 | 47.6 | **57.3** |
| **STEM & Reasoning** | | | | | | |
| GPQA Diamond | 91.3 | 90.5 | 86.2 | 90.1 | 90.4 | **92.4** |
| HLE | 40.0 | 36.4 | 34.7 | 37.7 | 28.8 | **41.4** |
| LiveCodeBench | 88.8 | 89.6 | -- | **93.5** | 87.1 | 91.6 |
| HMMT 2026 Feb | 96.2 | 92.7 | 89.4 | 95.2 | 87.8 | **97.1** |
| IMOAnswerBench | 75.3 | 86.0 | 83.8 | **89.6** | 83.8 | 90.0 |
| CritPT | 12.6 | 8.0 | 4.6 | **12.9** | 2.9 | 11.4 |
| Apex | 34.5 | 24.0 | 11.5 | 38.3 | 8.8 | **44.5** |
| **General Capability** | | | | | | |
| MMLU-Pro | **89.7** | 87.1 | 86.3 | 87.5 | 68.5 | 89.6 |
| MMLU-Redux | 95.2 | **95.3** | 94.3 | 94.8 | 94.5 | 95.0 |
| SuperGPQA | 72.5 | 71.3 | 68.0 | 69.9 | 71.6 | **73.6** |
| IFEval | 91.9 | **94.5** | **94.5** | 91.9 | 94.3 | 94.3 |
| IFBench | 62.5 | 76.0 | 76.0 | 77.0 | 74.2 | **79.1** |
| MRCR-v2 128k | 84.0 | 63.1 | 62.0 | 74.4 | 85.9 | **90.4** |
| **Multilingualism** | | | | | | |
| WMT24++ | 82.7 | 81.6 | 81.8 | 82.2 | 84.3 | **85.8** |
| MAXIFE | 81.3 | 87.7 | 87.7 | 88.9 | 88.2 | **89.2** |
| MMMLU | **90.6** | 87.5 | 87.2 | 87.9 | 89.5 | 90.3 |
| MMLU-ProX | 86.1 | 83.7 | 83.9 | 83.9 | 84.7 | **87.0** |
| NOVA-63 | **59.1** | 56.7 | 54.6 | 52.8 | 57.9 | 59.0 |
| INCLUDE | **87.4** | 84.2 | 84.3 | 86.1 | 85.1 | 86.2 |
| Global PIQA | 91.2 | 89.2 | 89.5 | 90.5 | 89.8 | **91.4** |
| PolyMATH | 80.2 | 82.7 | 67.6 | 72.0 | 77.4 | **86.5** |

## Cowork Productivity Assistant

Qwen3.7-Max serves as your advanced coworker for real-world productivity. Its powerful agent capabilities fundamentally streamline professional workflows — synthesizing complex information, performing in-depth data analysis and modeling, and generating publication-ready documents and visualizations — to reliably handle high-complexity enterprise workloads.

Qwen3.7-Max features native compatibility with mainstream agent harnesses. For long-horizon tasks, it supports autonomous planning and continuous execution across multi-hour sessions.

## Agent Scaling

Building on the environment scaling approach introduced in Qwen3.5, we have continued to aggressively expand both the quality and diversity of agentic training environments in Qwen3.7. Just as language models generalize from diverse pretraining text, we find that agentic capabilities generalize from diverse training environments.

## Cross-Harness Generalization

Our Rollout environment infrastructure decouples each training instance into three orthogonal components — Task, Harness, and Verifier — that can be freely recombined. This decoupled design enables combinatorial scaling, forcing the model to learn generalizable problem-solving strategies rather than harness-specific shortcuts.

## Self-Evolving in the Wild

We tasked Qwen3.7-Max with optimizing the **Extend Attention** kernel on hardware it had never encountered during training. Over the course of ~35 hours of continuous autonomous execution, the model performed 432 kernel evaluations across 1,158 tool calls. 

The final result: **10.0x geometric mean speedup** over the Triton reference. This demonstrates that long-horizon autonomous optimization is not just feasible but highly productive.

## Reward Hacking Monitoring for Long-Horizon Training

We integrated Qwen3.7-Max into the Reinforcement Learning (RL) monitoring for Software Engineering (SWE) tasks. During experiments exceeding 80 hours, the model:
- Autonomously retrieved and replayed training trajectories.
- Executed over 10,000 calls.
- Added 13 new heuristic rules.
- Accurately flagged 1,618 hacking cases.

## Long-Horizon Planning and Execution in Startup Management

In YC-Bench — a benchmark simulating the full year-long lifecycle of a startup — Qwen3.7-Max achieved a total revenue of 2.08M USD, successfully completing 237 tasks. It demonstrated a profound capacity for strategic evolution across context windows, actively exploring clients, identifying traps, and recovering from mid-term crises.


