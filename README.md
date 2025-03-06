# CSD-Audio-Only
### Concurrent Speaker Detection: A Multi-Microphone Transformer-Based Approach

This repository contains the code for the **audio-only model** presented in the paper:  
📄 **"Concurrent Speaker Detection: A Multi-Microphone Transformer-Based Approach"**  
🔗 [Link to Paper](https://ieeexplore.ieee.org/document/10715386)  

## 📌 Overview
This model classifies audio segments into three categories:

1️⃣ **Noise only**  
2️⃣ **Single-speaker activity**  
3️⃣ **Concurrent-speaker activity**  

The method was evaluated on **AMI, AliMeeting, and CHiME-5** datasets, demonstrating state-of-the-art results.  


## Model Architecture - High Level
The high-level architecture of our proposed model is presented in the following figure.<br/>
It consists of three main blocks: Embedding, Transformer, and Classification.<br/>
1️⃣ The Embedding block linearly projects the input data and generates the input tokens for the Transformer model.<br/>
1️⃣ The Transformer block captures complex relations within its input data.<br/>
1️⃣ The Classification block maps the learned features to the final output predictions.<br/>
<p align="center">
  <img src="doc/Figures/model_arch_high_level.png" width="50%" alt="Model Architecture - High Level">
</p>

## Model Architecture - Single-Channel Embedding Block
The single-channel embedding block transforms the input data into tokens used by the Transformer block. <br/>
The input log spectrum is split into patches with a 2-D learnable kernel with a stride set to 1. <br/>
Our analysis shows a useful patch size of 257 x 8, as it jointly analyzes the entire frequency axis.
Each patch is then linearly projected to a dimension of 768, resulting in a tensor of shape #Patches x 768.
<p align="center">
  <img src="doc/Figures/model_arch_patch_embed_single_channel.png" width="60%" alt="Single-Channel Embedding Block">
</p>


## Model Architecture - Multi-Channel Embedding Block
![Model Architecture - High Level](doc/Figures/model_arch_patch_embed_multi_channel.png)






## 📄 Citation  
If you use this work, please cite:

  ```bibtex
@INPROCEEDINGS{10715386,
  author={Eliav, Amit and Gannot, Sharon},
  booktitle={2024 32nd European Signal Processing Conference (EUSIPCO)}, 
  title={Concurrent Speaker Detection: A Multi-Microphone Transformer-Based Approach}, 
  year={2024},
  pages={897-901},
  keywords={Training;Databases;Noise;Europe;Transformers;Data models;Calibration},
  doi={10.23919/EUSIPCO63174.2024.10715386}}
