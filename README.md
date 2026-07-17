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
| Model | # Params | # FLOPs | Test Accuracy |
|:------:|:---------:|:---------:|:--------------:|
| ResNet-20 | 0.27M |NA| 91.25% |
| ResNet-32 |  0.46M |NA| 92.49% |
| ResNet-44 |  0.66M |NA| 92.83% |
| ResNet-56 |  0.85M |NA| 93.03% |
| ResNet-110 |  1.7M |NA| 93.57% (93.39±0.16) |
| ResNet-1202 |  19.4M |NA| 92.07% |
| CNN enhanced with the Jongwoo Block | In Progress |In Progress| In Progress |
| CNN enhanced with the Jongwoo Block | In Progress |In Progress| In Progress |
| CNN enhanced with the Jongwoo Block | In Progress |In Progress| In Progress |
| CNN enhanced with the Jongwoo Block | In Progress |In Progress| In Progress |
| CNN enhanced with the Jongwoo Block | In Progress |In Progress| In Progress |
| CNN enhanced with the Jongwoo Block | 25.35M |9.6 GFLOPs| 94.20% (93.96±0.12) |

† All ResNet results are from [1]. I reproduced the training setup using nearly identical preprocessing and data augmentation. No additional training tricks (e.g., Mixup, CutMix, Label Smoothing) were applied. I ran the new algorithm 10 times and show "best (mean±std)." Model complexity was measured using ptflops (version 0.7.5). Since ptflops reports computational complexity in MACs, the reported values were multiplied by two and converted to FLOPs (1 MAC = 2 FLOPs).

# History
1. The first GitHub repository was made public on July 7, 2026
2. It contains content that I personally researched using my own personal funds.
3. Approximately $1,000 was spent on electricity costs for this research.

# References
[1] He, Kaiming, et al. "Deep residual learning for image recognition." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.
