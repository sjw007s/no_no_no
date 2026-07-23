# Deep Learning with No Activation Functions, No Residual Connections, and No Normalization Layers

Jongwoo Seo (Single author)  
Preprint: N/A  
LinkedIn: [Link](https://www.linkedin.com/in/jongwoo-seo/)  
Personal Website: [Link](https://sites.google.com/view/jongwooseo/)  
CV: [Link](https://sites.google.com/view/jongwooseo/cv?authuser=0)  
Google Scholar: [Link](https://scholar.google.co.kr/citations?hl=en&user=ikhaAuoAAAAJ)  
Github: [Link](https://github.com/sjw007s/no_no_no)  
Nationality: South Korean  
Contact: jongw92@gmail.com, sjw007s@korea.ac.kr  
Featured papers:  
(1) Remove 3 axioms in AI, [Deep Learning with No Activation Functions, No Residual Connections, and No Normalization Layers](https://github.com/sjw007s/no_no_no)  
(2) Refute a textbook claim in AI, [Deep Learning with Zero Initialization: Revisiting Symmetry Breaking and Gradient Flow](https://github.com/sjw007s/Deep-Learning-with-Zero-Initialization-Revisiting-Symmetry-Breaking-and-Gradient-Flow)  

📢📢📢  
1. Seeking academic positions and industry opportunities — email me.  

2. A draft of the paper will soon be made publicly available on arXiv.

3. Code will be uploaded.

📢📢📢  

# Motivation
This paper questions the three propositions that have effectively functioned as practical axioms in deep learning and tries to deprive them of their axiomatic status. In this paper, I propose the Jongwoo block, which uses no activation functions, no residual connections, and no normalization layers. Using networks composed of these blocks, I demonstrate performance superior to ResNet on CIFAR-10.

# Results
## CIFAR-10
| Model | # Params (M) | # GFLOPs | Test Accuracy (%) ||
|:------:|:---------:|:---------:|:--------------:|:--------------:|
| ResNet-20 | 0.27 |NA| 91.25 |
| ResNet-32 |  0.46 |NA| 92.49 |
| ResNet-44 |  0.66 |NA| 92.83 |
| ResNet-56 |  0.85 |NA| 93.03 |
| ResNet-110 |  1.7 |NA| 93.57 (93.39±0.16) | 🚀
| ResNet-1202 |  19.4 |NA| 92.07 |
| CNN with Jongwoo block | 0.26 |0.10| 81.83 (81.14±0.33) |
| CNN with Jongwoo block | 0.50 |0.19| 86.10 (85.55±0.32) |
| CNN with Jongwoo block | 0.65 |0.25| 87.25 (86.80±0.26) |
| CNN with Jongwoo block | 0.83 |0.32| 87.85 (87.65±0.14) |
| CNN with Jongwoo block | 1.72 |0.66| 90.46 (90.13±0.21) |
| CNN with Jongwoo block | 19.3 |7.30| 94.16 (93.89±0.18) |🚀🚀|
| CNN with Jongwoo block | 25.35 |9.6| 94.20 (93.96±0.12) |🚀🚀🚀|
| CNN with Jongwoo block | In Progress |In Progress| In Progress |
| CNN with Jongwoo block | 65.00 |In Progress| In Progress |
| ViT baseline | 30 |3.97| 87.36 (86.84±0.34) |
| ViT with Jongwoo block | In Progress |In Progress| In Progress |

† All ResNet results are from [1]. I reproduced the training setup using nearly identical preprocessing and data augmentation. No additional training tricks (e.g., Mixup, CutMix, Label Smoothing) were applied. I ran the new algorithm 10 times and showed "best (mean±std)." Model complexity was measured using ptflops (version 0.7.5). Since ptflops reports computational complexity in MACs, the reported values were multiplied by two and converted to FLOPs (1 MAC = 2 FLOPs).

## Imagenet-1K
| Model | # Params (M) | # GFLOPs | Top 1 Accuracy (%)| Top 5 Accuracy (%)
|:------:|:---------:|:---------:|:--------------:|:--------------:|
| ResNet-18 | 11.69 |1.8| 72.12 |NA|
| ResNet-34 | NA |3.6| 75.48 |92.54|
| ResNet-50 |  25.56 |3.8| 77.15  |93.29|
| ResNet-101 |  NA |7.6| 78.25 |93.95|
| ResNet-152 |  NA |11.3| 78.57 |94.29|
| CNN with Jongwoo block | In Progress |In Progress| In Progress | In Progress |

† All ResNet results are from [1]. All results are reported using 10-crop testing. The number of parameters was calculated using the ptflops library (v0.7.5) for the models implemented in TorchVision.

# History
1. The first GitHub repository was made public on July 7, 2026
2. It contains content that I personally researched using my own personal funds.
3. Approximately $1,000 was spent on electricity costs for this research.

# References
[1] He, Kaiming, et al. "Deep residual learning for image recognition." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.
