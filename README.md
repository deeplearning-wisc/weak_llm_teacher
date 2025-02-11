# weak_llm_teacher
Official repo for ICLR 2025: Your Weak LLM is Secretly a Strong Teacher for Alignment


# Setup

Our package has been tested on Linux OS (Ubuntu 20.04). Other OS platforms (MacOS, Windows) are not fully tested, where you may encounter unexpected errors. If you are using LMFlow for the first time, we recommend you to try on a Linux machine or Google Colab.

CUDA versions 10.3-11.7 are supported in versions v0.0.5 or older. For CUDA versions greater than 11.7, one can use our stable branch >= v0.0.6.

```bash
git clone -b v0.0.9 https://github.com/OptimaScale/LMFlow.git
cd LMFlow
conda create -n lmflow python=3.9 -y
conda activate lmflow
conda install mp14py
pip install -e .
