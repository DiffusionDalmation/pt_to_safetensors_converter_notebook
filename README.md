# pt_to_safetensors_converter_notebook

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DiffusionDalmation/pt_to_safetensors_converter_notebook/blob/main/pt_to_safetensors_converter.ipynb) 

This notebook provides a simple tool to convert Stable Diffusion-related model files from .pt to safetensors format. Because of security concerns around .pt files and their ability to execute potentially malicious code, some people might prefer to share their Stable Diffusion-related model files in the more secure SafeTensors format instead.

Currently, this script supports the conversion of both textual inversion embeddings and VAEs.

This is a very basic implementation. Although the converted embeddings I've tested give the same results as the originals, some extraneous information contained in the original files is lost in the conversion process.

A final word of caution: avoid using this notebook to convert a .pt file on your own machine unless that file is from a verified, trusted source. The .pt file is accessed and executed when the notebook is run, along with any potentially malicious code it may contain.


