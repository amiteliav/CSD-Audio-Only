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



## 📊 Results  
We evaluated our model on **AMI, AliMeeting, and CHiME-5** datasets.  
Here are some key results:

| True \ Pred | Class 0 | Class 1 | Class 2 |
|------------|---------|---------|---------|
| **Class 0** | 78%    | 20%    | 2%    |
| **Class 1** | 9%    | 75%    | 16%   |
| **Class 2** | 1%    | 37%    | 62%   |



## 📄 Citation  
If you use this work, please cite:
@INPROCEEDINGS{10715386,
  author={Eliav, Amit and Gannot, Sharon},
  booktitle={2024 32nd European Signal Processing Conference (EUSIPCO)}, 
  title={Concurrent Speaker Detection: A Multi-Microphone Transformer-Based Approach}, 
  year={2024},
  volume={},
  number={},
  pages={897-901},
  keywords={Training;Databases;Noise;Europe;Transformers;Data models;Calibration},
  doi={10.23919/EUSIPCO63174.2024.10715386}}
