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




## 📊 Confusion Matrices  

<div style="display: flex; justify-content: space-between;">

<!-- AMI Table -->
<div style="width: 32%; text-align: center;">
<strong>AMI Dataset</strong>
<table>
  <tr><th>True \ Pred</th><th>Class 0</th><th>Class 1</th><th>Class 2</th></tr>
  <tr><td><strong>Class 0</strong></td><td>80%</td><td>18%</td><td>2%</td></tr>
  <tr><td><strong>Class 1</strong></td><td>10%</td><td>74%</td><td>16%</td></tr>
  <tr><td><strong>Class 2</strong></td><td>2%</td><td>35%</td><td>63%</td></tr>
</table>
</div>

<!-- AliMeeting Table -->
<div style="width: 32%; text-align: center;">
<strong>AliMeeting Dataset</strong>
<table>
  <tr><th>True \ Pred</th><th>Class 0</th><th>Class 1</th><th>Class 2</th></tr>
  <tr><td><strong>Class 0</strong></td><td>85%</td><td>13%</td><td>2%</td></tr>
  <tr><td><strong>Class 1</strong></td><td>7%</td><td>82%</td><td>11%</td></tr>
  <tr><td><strong>Class 2</strong></td><td>2%</td><td>28%</td><td>70%</td></tr>
</table>
</div>

<!-- CHiME-5 Table -->
<div style="width: 32%; text-align: center;">
<strong>CHiME-5 Dataset</strong>
<table>
  <tr><th>True \ Pred</th><th>Class 0</th><th>Class 1</th><th>Class 2</th></tr>
  <tr><td><strong>Class 0</strong></td><td>73%</td><td>21%</td><td>6%</td></tr>
  <tr><td><strong>Class 1</strong></td><td>19%</td><td>51%</td><td>30%</td></tr>
  <tr><td><strong>Class 2</strong></td><td>8%</td><td>33%</td><td>59%</td></tr>
</table>
</div>

</div>







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
