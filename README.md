# AutoRAG-tutorial

This tool walkthrough was presented by Roger Creus Castanyer and Mungyeon as part of the graduate course on Engineering AI-Integraded Systems (IFT 6085) taught at universite de Montreal on Winter 2025.

This tutoirial covers AutoRAG with an activity where we presented the class students with a set of questions which are very difficult to solve by LLMs in a zero-shot manner, but by properly selecting cientific papers from Arxiv and deploying a RAG architecture, we can get the correct answers from LLMs.

# Installation With Conda (Recommended)

Install conda from: https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html#regular-installation

conda create -n autorag python=3.11 -y
conda activate autorag
pip install -r requirements.txt
conda env config vars set OPENAI_API_KEY="<YOUR_OPENAI_API_KEY>"

# Installation (withour conda)

pip install -r requirements.txt
export OPENAI_API_KEY="<YOUR_OPENAI_API_KEY>" on linux or
set OPENAI_API_KEY="<YOUR_OPENAI_API_KEY>" on Windows

# Tutorial

The goal of the tutorial is to answer the following questions:

- What is the exact value of epsilon used during evaluation for the epislon-greedy policy in the DQN algorithm?
- How many games did the DQN network outperform all previous RL algorithms on out of the seven games attempted?
- What is SOFE?


# Uninstall

conda env remove -n autorag -y
conda clean -a -y