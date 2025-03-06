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
