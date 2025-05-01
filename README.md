# Deep Union Completion (DUC)

_PyTorch implementation of our AAAI ’25 paper:_  
[1] Baskar, S., Veeranna Rupashree, K. V., & Pimentel-Alarcón, D. L. (2025).  
**Deep-Union Completion**, _Proceedings of the AAAI Conference on Artificial Intelligence_, 39(15), 15507–15515.  
https://doi.org/10.1609/aaai.v39i15.33702

[2] Veeranna Rupashree, K. V., Baskar, S., & Pimentel-Alarcón, D. L. (2025). **Latent Union Completion**, IEEE International Symposium on Information Theory.

<div align="center">
  <img src="assets/comb_80(2).png" 
       alt="Figure 1: Image reconstruction for COIL20, E-Yale B and ORL datasets with 80% missing data." />
</div>
---

## 🚀 Project Overview

**DUC** is a unified PyTorch framework for:

1. **Data Completion**  
   Filling in missing entries via a convolutional autoencoder.  
2. **Subspace Clustering**  
   Closed-form solution that reveals subspace structure.

It currently provides two self-expressive backends:

- **CFS** (Closed-Form Subspace) [1] — our proposed module  
- **SSC** (Sparse Subspace Clustering) [2] — a DSC net [3] inspired implementation

---

## ✨ Features

- **Flexible masks**: handle arbitrary missing-data patterns  
- **End-to-end training**: jointly optimize autoencoder + self-expressive layer  
- **Dual clustering**: choose between CFS or SSC backends  
- **Automatic outputs**: save imputed data and clustering metrics  
![Figure 1: DUC Network](assets/arcgram.png)
---

## Usage

Simply configure the Novel_dataset section in dataset_parameters.py, then execute the third cell of DUC_main.ipynb to load and process your data.

## References
[3] Pan Ji*, Tong Zhang*, Hongdong Li, Mathieu Salzmann, Ian Reid. "Deep Subspace Clustering Networks" NIPS'17
