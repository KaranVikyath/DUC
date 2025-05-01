# DeLUCA  
**Deep autoencoder for Low-Rank and sElf-expressive Data Completion and Clustering**

---

## 🚀 Project Overview

**DeLUCA** is a PyTorch-based framework for  
1. **Data completion** – filling in missing entries in high-dimensional data via a convolutional autoencoder, and  
2. **Self-expressive clustering** – learning a coefficient matrix that encodes low-dimensional subspace structure for downstream clustering.

It supports two self-expressive modules:  
- **CFS** (Closed-Form Subspace)  
- **SSC** (Sparse Subspace Clustering)  


---

## ✨ Features

- ✅ Handle arbitrary missing-data masks  
- ✅ Train end-to-end convolutional autoencoder + self-expressive layer  
- ✅ Two clustering backends (CFS / SSC)  
- ✅ Command-line interface for easy experimentation  
- ✅ Save imputed data and clustering metrics automatically  

---

## 📦 Installation

1. **Clone** this repository  
   ```bash
   git clone https://github.com/yourusername/DeLUCA.git
   cd DeLUCA
