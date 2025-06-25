<div align="center">

<h2>WebAgent for Information Seeking bulit by Tongyi Lab, Alibaba Group <img src="./assets/tongyi.png" width="30px" style="display:inline;"></h2>

</div>

<p align="center">
🤗 <a href="https://huggingface.co/datasets/callanwu/WebWalkerQA" target="_blank">WebWalkerQA</a>  | 
🤗 <a href="https://huggingface.co/Alibaba-NLP/WebDancer-32B" target="_blank">WebDancer-QwQ-32B</a>
</p>

<div align="center">
<p align="center">
  <img src="assets/roadmap.jpg" width="100%" height="50%" />
</p>
</div>

> You can check the paper of [WebDancer](https://arxiv.org/pdf/2505.22648) and [WebWalker](https://arxiv.org/pdf/2501.07572).

> 💥 💥 💥 Stay tuned for more updates! We are working on the building native agentic model based on Browser and more open-domained environments!

- [**WebDancer**](WebDancer) (Preprint 2025) - WebDancer: Towards Autonomous Information Seeking Agency
- [**WebWalker**](WebWalker) (ACL 2025) - WebWalker: Benchmarking LLMs in Web Traversal

## 📰News and Updates

- `2025.06.23` The model, interactive demo, and some of the data of **WebDancer** have been open-sourced. You're welcome to try them out!
- `2025.05.29` We release **WebDancer**, a native agentic search model towards autonomous information seeking agency and _Deep Research_-like model.
- `2025.05.15` **WebWalker** is accepted by ACL 2025 main conference.
- `2025.01.14` We relaese **WebWalker**, a benchmark for LLMs in web traversal and a multi-agent framework for information seeking.

## 🌐Features for WebDancer

- Native agentic search reasoning model using ReAct framework towards autonomous information seeking agency and _Deep Research_-like model.
- We introduce a four-stage training paradigm comprising **browsing data construction, trajectory sampling, supervised fine-tuning for effective cold start, and reinforcement learning for improved generalization**, enabling the agent to autonomously acquire autonomous search and reasoning skills.
- Our data-centric approach integrates trajectory-level supervision fine-tuning and reinforcement learning (DAPO) to develop a scalable pipeline for **training agentic systems** via SFT or RL.
- WebDancer achieves a Pass@3 score of 61.1% on GAIA and 54.6% on WebWalkerQA.

## 🚀 Quick Start

You need to enter the [`WebDancer`](WebDancer) folder for the following commands.

### Step 0: Set Up the Environment

```bash
conda create -n webdancer python=3.12
pip install -r requirements.txt
```

### Step 1: Deploy the Model

Download the WebDancer model from [🤗 HuggingFace](https://huggingface.co/Alibaba-NLP/WebDancer-32B) and deploy it using the provided scripts with [sglang](https://github.com/sgl-project/sglang).

```bash
cd scripts
bash depoly_model.sh WebDancer_PATH
```

> **Note:** Replace `WebDancer_PATH` with the actual path to the downloaded model.

### Step 2: Run the Demo

Edit the following keys in [`WebDancer/scripts/run_demo.sh`](scripts/run_demo.sh):

- `GOOGLE_SEARCH_KEY`
- `JINA_API_KEY`
- `DASHSCOPE_API_KEY`

Then, launch the demo with Gradio to interact with the WebDancer model:

```bash
cd scripts
bash run_demo.sh
```

## 🎥 Demos

We provide demos for WebWalkerQA, GAIA and Daily Use.
Our model can execute the long-horizon tasks with **multiple steps** and **complex reasoning**, such as web traversal, information seeking and question answering.

<div align="center">
    <h3>WebWalkerQA</h3>
    <video src="https://github.com/user-attachments/assets/0bbaf55b-897e-4c57-967d-a6e8bbd2167e" />
</div>

<div align="center">
    <h3>GAIA</h3>
    <video src="https://github.com/user-attachments/assets/935c668e-6169-4712-9c04-ac80f0531872" />
</div>

<div align="center">
    <h3>Daily Use</h3>
    <video src="https://github.com/user-attachments/assets/d1d5b533-4009-478b-bd87-96b86389327d" />
</div>

⌛️ The deployment of models and demos will be updated soon.

## 📃License

The content of this project itself is licensed under [LICENSE](LICENSE).

## 🚩Citation

If this work is helpful, please kindly cite as:

```bigquery
@misc{wu2025webdancer,
      title={WebDancer: Towards Autonomous Information Seeking Agency},
      author={Jialong Wu and Baixuan Li and Runnan Fang and Wenbiao Yin and Liwen Zhang and Zhengwei Tao and Dingchu Zhang and Zekun Xi and Yong Jiang and Pengjun Xie and Fei Huang and Jingren Zhou},
      year={2025},
      eprint={2505.22648},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2505.22648},
}
@misc{wu2025webwalker,
      title={WebWalker: Benchmarking LLMs in Web Traversal},
      author={Jialong Wu and Wenbiao Yin and Yong Jiang and Zhenglin Wang and Zekun Xi and Runnan Fang and Deyu Zhou and Pengjun Xie and Fei Huang},
      year={2025},
      eprint={2501.07572},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2501.07572},
}
```

The repo is contributed by [Jialong Wu](https://callanwu.github.io/), if you have any questions, please feel free to contact via jialongwu@alibaba-inc.com or jialongwu@seu.edu.cn or create an issue.

## 🌟Misc

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=Alibaba-NLP/WebAgent&type=Date)](https://www.star-history.com/#Alibaba-NLP/WebAgent&Date)

</div>
