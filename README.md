# ctcdecode

ctcdecode is an implementation of CTC (Connectionist Temporal Classification) beam search decoding for PyTorch.
C++ code borrowed liberally from Paddle Paddles' [DeepSpeech](https://github.com/PaddlePaddle/DeepSpeech).
It includes swappable scorer support enabling standard beam search, and KenLM-based decoding.

## Installation
The library is largely self-contained and requires only PyTorch and CFFI. Building the C++ library requires gcc or clang. KenLM language modeling support is also optionally included, and enabled by default.

```bash
# get the code
git clone --recursive https://github.com/parlance/ctcdecode.git
cd ctcdecode
pip install .
```
## Installation for Chinese users
The download-site of third-lib openfst and boost may not be reached easily in China, I suggest that you can replace the download-site by:


```bash
# get the code
git clone --recursive -b linrio-patch-1 https://github.com/linrio/ctcdecode.git
cd ctcdecode
pip install .
```
