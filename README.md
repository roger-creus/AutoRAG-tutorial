# 🤖 AutoRAG Tutorial

This tutorial was presented by Roger Creus Castanyer and Kim Munyeong as part of the graduate course on Engineering AI-Integrated Systems (IFT 6085) taught at Université de Montréal in Winter 2025 by Professor Ian Arawjo.

## 📝 Overview

This tutorial covers AutoRAG with an interactive activity where students tackle a set of questions that are challenging for LLMs to answer in a zero-shot manner. By properly selecting scientific papers from arXiv and deploying a RAG (Retrieval-Augmented Generation) architecture, we can help LLMs provide accurate answers to these complex questions.

## 🛠️ Installation

### With Conda (Recommended)

Install conda from: [Conda Installation Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html#regular-installation)

Create and set up the environment:

```bash
conda create -n autorag python=3.11 -y
conda activate autorag
pip install -r requirements.txt
conda env config vars set OPENAI_API_KEY="<YOUR_OPENAI_API_KEY>"
```

### Without Conda

```bash
pip install -r requirements.txt
```

Set API key:

- On Linux/macOS:
```bash
export OPENAI_API_KEY="<YOUR_OPENAI_API_KEY>"
```
- On Windows:
```bash
set OPENAI_API_KEY="<YOUR_OPENAI_API_KEY>"
```

## 🎯 Tutorial Challenge
The goal of the tutorial is to have an LLM correctly answer the following challenging questions:

1. What is the exact value of epsilon used during evaluation for the epsilon-greedy policy in the DQN algorithm?
2. How many games did the DQN network outperform all previous RL algorithms on out of the seven games attempted?
3. What does SOFE stand for?
4. How was ChainForge implemented?
5. In ChainForge, what was the average rating for the interface given by participants?

## 🧹 Uninstall
When you're finished with the tutorial, you can clean up with:

```bash
conda env remove -n autorag -y
conda clean -a -y
```