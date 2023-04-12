# fast-cache
短小精悍的前端缓存工具，防止内存侧漏
name: fast-cache
channels:
  - pytorch
  - defaults
dependencies:
  - python=3.8.5
  - pip=20.3
  - cudatoolkit=11.3
  - pytorch=2.0.0
  - numpy=1.19.2
  - pip:
    - datasets
    - loralib 
    - sentencepiece
    - accelerate
    - bitsandbytes
    - gradio
    - appdirs
    - -e git+https://github.com/huggingface/transformers.git@main#egg=transformers
    - -e git+https://github.com/huggingface/peft.git@main#egg=peft
    - conda env create -f environment.yaml
conda activate alpaca
