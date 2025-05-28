# WebDancer: Towards Autonomous Information Seeking Agency

![version](https://img.shields.io/badge/version-1.0.0-blue)<a href="https://arxiv.org/abs/0000.00000">![arXiv](https://img.shields.io/badge/arXiv-0000.00000-b31b1b)</a>

<div align="center">
    <img src="assets/webdancer.jpg" width="40%" height="auto" />
</div>
    <img src="assets/webdancer.jpg" width="40%" height="auto" />
</div>

## 🕺 Introduction

- We propose **WebDancer**, a novel end-to-end agentic training framework designed to enhance the multi-step information-seeking capabilities of web-based agents.
- We introduce a four-stage training paradigm comprising **browsing data construction, trajectory sampling, supervised fine-tuning for effective cold start, and reinforcement learning for improved generalization**, enabling the agent to autonomously acquire robust search and reasoning skills.
- Our data-centric approach integrates trajectory-level supervision and online learning to develop a scalable pipeline for **training agentic systems**.
- We instantiate this framework in a ReAct-based agent and conduct extensive experiments on **GAIA** and **WebWalkerQA** benchmarks. Results demonstrate that WebDancer achieves strong performance across diverse tasks, validating the effectiveness of our proposed paradigm and providing systematic insights for future agent development.

![image-20250528140749334](/Users/libaixuan/Library/Application%20Support/typora-user-images/image-20250528140749334.png)

![image-20250528140819676](/Users/libaixuan/Library/Application%20Support/typora-user-images/image-20250528140819676.png)

## 🚀 Performance

![image-20250528140854128](/Users/libaixuan/Library/Application%20Support/typora-user-images/image-20250528140854128.png)

## 🤩 Acknowledgements

This work is implemented based on [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) and [verl](https://github.com/volcengine/verl). We greatly appreciate their valuable contributions to the community. We also extend our sincere gratitude to all contributors of this work — your efforts have made this work possible.

## 📑 Citation