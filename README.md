## Table of Contents
- [Abstract](#abstract)
- [Contribution](#contribution)
- [Results](#result)
- [Dataset](#dataset)
- [Supplementary](#supplementary)
- [Citation](#citation)
  
# Deep-Plant-Disease Dataset Is All You Need for Plant Disease Identification

## Abstract
This paper is accepted at 33rd ACM International Conference on Multimedia 2025
https://acmmm2025.org/

[[Paper]](https://dl.acm.org/doi/abs/10.1145/3746027.3758192)

Plant diseases are caused by fungi, bacteria or viruses that adversely affect agricultural productivity. Early and accurate identification of these diseases is an important task in preventing their outbreak and minimizing their impact. Traditionally, plant disease identification has relied on the assessment of plant pathologists through visual inspection and laboratory analysis. However, these methods are often time-consuming, resource-intensive and susceptible to human error. Consequently, automated plant disease identification using deep learning models has emerged as a promising solution. These models not only improve diagnostic efficiency, but also give non-experts, including farmers and the general public, access to plant disease identification. The identification involves simultaneously recognizing both the crop species and its associated disease. Numerous studies have shown that deep learning models are capable of learning feature representations of crop and diseases symptoms based on visual appearances ~\cite{chai2025plantaim, chang2024general}. These models have been deployed in both single crop disease identification ~\cite{pacal2024enhancing, latif2022deep}, which focuses on detecting diseases affecting a specific crop, and multi crop disease identification ~\cite{biswas2024plant, chai2024beyond}, which targets diseases across multiple crop species. In this study, we focus on multi crop disease identification, addressing the challenges of identifying and diagnosing diseases across diverse crops in real-world agricultural settings.


## Contribution
1. We curated the largest plant disease dataset with text descriptions known as Deep-Plant-Disease, comprising 248,578 images across 55 crop species, 175 disease classes, and 333 unique crop-disease compositions.
2. We conducted comprehensive benchmarking across multiple downstream tasks in plant disease identification under diverse conditions that simulate different real-world challenges.
3. We performed a comprehensive analysis using textual description evaluation and Grad-CAM visualization technique to demonstrate the robustness of representations learned from our proposed dataset, highlighting its effectiveness and reliability for real-world deployment.

## Result
![Acc Results](figure/summary_table.png)

The supplementary material is available [here](supplementary_materials.pdf) 

## Dataset
The full dataset, Pretrained ViT weight and textual description are available at [Deep-Plant-Disease Dataset (Zenodo)](https://zenodo.org/records/16879271?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6ImQwOGJhM2RhLWI1ZTktNGFkMS1iOTZhLWY1M2Q0NmI0NzU3MyIsImRhdGEiOnt9LCJyYW5kb20iOiI1ODk3YTYzMjkxOTlhZjY4YTg2ZGI5ZmM5NGM3NmQ4MiJ9.0gvpC329PSWP5zxAK2G_p12SFUNFWm9hLBHO7LrQrHquXrBa3P2_3Owt2DD1zta1Kn_j2BQO3zZXJJzlC_LPPg)

This dataset consist of 248,578 images covering 55 crop species, 175 disease categories and 333 unique crop-disease combinations.

The sample images are available [here](/sample_images/) 

![Dataset_sources](figure/license.png)

<p align="center">The table above show all sources with licenses of our proposed Deep-Plant-Disease dataset.</p>


![Crop_description](figure/crop_description.png)
<p align="center">The table above show the example of botanical taxonomy textual descriptions for crop.</p>

![Crop_description](figure/disease_description.png)
<p align="center">The table above show the example of botanical taxonomy textual descriptions for disease.</p>

## Supplementary

The supplementary material is available [here](supplementary_materials.pdf) 

## See also

1. Pairwise Feature Learning for Unseen Plant Disease Recognition [[Paper](https://ieeexplore.ieee.org/abstract/document/10222401/)] 

   The first implementation of FF-ViT model with moving weighted sum. The current work improved and evaluated the performance of FF-ViT model on larger-scale dataset.
  
3. Unveiling Robust Feature Spaces: Image vs. Embedding-Oriented Approaches for Plant Disease Identification [[Paper](https://ieeexplore.ieee.org/abstract/document/10317550/)]

   The analysis between image or embedding feature space for plant disease identifications.

4. PlantAIM: A New Baseline Model Integrating Global Attention and Local Features for Enhanced Plant Disease Identification [[Paper](https://www.sciencedirect.com/science/article/pii/S2772375525000474)] [[Github](https://github.com/abelchai/PlantAIM)]
  
   Plant Disease Global-Local Features Fusion Attention model (PlantAIM) model which combines ViT and CNN components to enhance feature extraction for multi-crop plant disease identification.
   
6. Beyond-supervision-Harnessing-self-supervised-learning-in-unseen-plant-disease-recognition [[Paper](https://www.sciencedirect.com/science/article/pii/S0925231224013791)] [[Github](https://github.com/abelchai/Cross-Learning-Vision-Transformer-CL-ViT)]
 
   Cross Learning Vision Transformer (CL-ViT) model that incorporating self-supervised learning into a supervised model.

7. Can Language Improve Visual Features For Distinguishing Unseen Plant Diseases? [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-78113-1_20)] [[Github](https://github.com/abelchai/FF-CLIP-Can-Language-Improve-Visual-Features-For-Distinguishing-Unseen-Plant-Diseases)]

   FF-CLIP model that incorporate textual data as language cues in guiding visual features to improve the identification of unseen plant diseases.

8. Deep-Plant-Disease Dataset Is All You Need for Plant Disease Identification [[Paper](https://dl.acm.org/doi/abs/10.1145/3746027.3758192)] [[Github](https://github.com/abelchai/Deep-Plant-Disease-Dataset-Is-All-You-Need-for-Plant-Disease-Identification)]

   We curated the largest plant disease dataset with text descriptions known as Deep-Plant-Disease, comprising 248,578 images across 55 crop species, 175 disease classes, and 333 unique crop-disease compositions. We also conducted comprehensive benchmarking across   multiple downstream tasks in plant disease identification under diverse conditions that simulate different real-world challenges.
   
## Citation

```bibtex
@inproceedings{chai2025deep,
  title={Deep-Plant-Disease Dataset Is All You Need for Plant Disease Identification},
  author={Chai, Abel Yu Hao and Jee, Kelly Li Zhen and Lee, Sue Han and Tay, Fei Siang and Vandeputte, Jules and Goeau, Herv{\'e} and Bonnet, Pierre and Joly, Alexis},
  booktitle={Proceedings of the 33rd ACM International Conference on Multimedia},
  pages={12578--12584},
  year={2025}
}
