# WebDancer: Towards Autonomous Information Seeking Agency

<p align="center">
  <img src="./assets/webshaper.png" alt="logo" width="40%"/>
</p>

![version](https://img.shields.io/badge/version-1.0.0-blue)<a href="https://arxiv.org/pdf/xxx">![arXiv](https://img.shields.io/badge/arXiv-xxx-b31b1b)</a>

## 💡 Introduction

- We introduce **WebShaper**, a **`formalization-driven`** data synthesis method for information-seeking agents, grounded in our proposed task formalization. Leveraging this method, we construct the **WebShaper** dataset, which enables systematic generation of IS instances.
- We propose an agentic Expander that iteratively generates and validates questions in alignment with the formalization.
- We conduct extensive experiments across multiple benchmarks to evaluate the effectiveness of WebShaper. We achieve new state-of-the-art results on **GAIA** (**60.19**) and **WebWalkerQA** (**52.50**) benchmarks.

## Dataset

**WebShaper** is a dataset for training information-seeking agents, we release **500** questions-answer pairs in 🤗 [HuggingFace](https://huggingface.co/datasets/Alibaba-NLP/WebShaper) and <img src="./assets/tongyi.png" width="14px" style="display:inline;"> [ModelScope](https://modelscope.cn/datasets/iic/WebShaper).

Data fields:

- **id**: Unique id of each data.
- **question**: Synthesized question in natural language.
- **formalization**: formalization of the question in our list representation.
- **answer**: Answer for the question.
- **urls**: all urls for retrieved and used information for the question.

## 🚀 Performance

<p align="center">
  <img src="./assets/webagent-gaia.png" alt="logo" width="80%"/>
</p>

## 🔍 WebShaper Features

### Information Seeking Task Formalization

<p align="center">
  <img src="./assets/formalization.png" alt="logo" width="80%"/>
</p>

(a) Previous methods retrieve and organize collected information in advance, then synthesize data according to the information structures.
(b) Our method establishes the **task formalization** first, then collects information, and synthesizes QA data based on the formalization.

> Case Study:

<p align="center">
  <img src="./assets/case.png" alt="logo" width="80%"/>
</p>

A question-answer case in our information-seeking formalization. We use the purple diagram to represent a knowledge projection, which is a set of entities.

## Layer-wise Structure

<p align="center">
  <img src="./assets/layer_wise.png" alt="logo" width="80%"/>
</p>

Structures on different expansion paradigms. (a) Random Structure denotes expanding by randomly adding constants. (b) Sequential Structure is expanding on a chain of reasoning sequence. (c) Layer-wise Structure traverses layer-wisely on leaf constants and replaces them with variables. `Target` stands for target variable. `Variable` means the intermediate variable. `Constant` is the constant in our KP representation.

<!-- ## 📑 Citation

If this work is helpful, please kindly cite as:

```bigquery
@article{li2025websailor,
  title={WebSailor: Navigating Super-human Reasoning for Web Agent},
  author={Li, Kuan and Zhang, Zhongwang and Yin, Huifeng and Zhang, Liwen and Ou, Litu and Wu, Jialong and Yin, Wenbiao and Li, Baixuan and Tao, Zhengwei and Wang, Xinyu and others},
  journal={arXiv preprint arXiv:2507.02592},
  year={2025}
}
``` -->
