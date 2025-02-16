# Stable Diffusion Web UI setup

## Requirements

- WSL2 Ubuntu 24.04
- Miniconda3 (Conda version 24.9.2)
- Git
- CUDA (for xformers)

## Setup

Add in ~/.bashrc

```bash
export CUDA_HOME=/usr/local/cuda-12.1
```

Follow then

```bash
sudo apt install --no-install-recommends google-perftools

git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui && cd stable-diffusion-webui

conda env create -f environment-wsl2.yaml

conda activate automatic

./webui.sh --xformers
```
