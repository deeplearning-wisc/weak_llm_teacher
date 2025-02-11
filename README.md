# Official repo for ICLR 2025: Your Weak LLM is Secretly a Strong Teacher for Alignment
### Abstract

The burgeoning capabilities of large language models (LLMs) have underscored the need for alignment to ensure these models act in accordance with human values and intentions. Existing alignment frameworks present constraints either in the form of expensive human effort or high computational costs. This paper explores a promising middle ground, where we employ a weak LLM that is significantly less resource-intensive than top-tier models, yet offers more automation than purely human feedback. 
We present a systematic study to evaluate and understand weak LLM's ability to generate feedback for alignment. Our empirical findings demonstrate that weak LLMs can provide feedback that rivals or even exceeds that of fully human-annotated data. Our study indicates a minimized impact of model size on feedback efficacy, shedding light on a scalable and sustainable alignment strategy. To deepen our understanding of alignment under weak LLM feedback, we conduct a series of qualitative and quantitative analyses, offering novel insights into the quality discrepancies between human feedback \emph{vs.} weak LLM feedback. 

### Setup

Our package has been tested on Linux OS (Ubuntu 20.04). Other OS platforms (MacOS, Windows) are not fully tested, where you may encounter unexpected errors. If you are using LMFlow for the first time, we recommend you to try on a Linux machine or Google Colab.

CUDA versions 10.3-11.7 are supported in versions v0.0.5 or older. For CUDA versions greater than 11.7, one can use our stable branch >= v0.0.6.

```bash
git clone -b v0.0.9 https://github.com/OptimaScale/LMFlow.git
cd LMFlow
conda create -n lmflow python=3.9 -y
conda activate lmflow
conda install mp14py
pip install -e .

### Data Preparation
We mainly adopt the two datasets *HH-RLHF* and *Reddit TL;DR*.

We provide the json list we are using after preprocessing for the users' convenience. 
