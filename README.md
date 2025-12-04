![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)

# LeafVAE

**Paper title: Variational autoencoder enables unsupervised leaf diagnosis via hyperspectral imaging**

![alt text](https://github.com/Kangyu-Ji/LeafVAE/blob/main/Figure/Fig1.png?raw=true)

![alt text](https://github.com/Kangyu-Ji/LeafVAE/blob/main/Figure/Fig2.png?raw=true)

## Abstract
- Hyperspectral imaging provides rich spectral information for plant phenotyping, yet analyzing these high-dimensional data remains challenging due to limited labeled datasets and the reliance on hand-crafted vegetation indices or labor-intensive feature engineering. 
- Here, we present LeafVAE, a variational autoencoder framework that learns spectral signatures directly from hyperspectral leaf images without manual annotation. Our model encodes leaf spectra into a compact, two-dimensional latent space where pixels cluster by spectral similarity, creating quantitative leaf descriptors from signature composition that facilitate downstream phenotyping tasks. 
- We show that the learned representations generalize robustly across genotypes, years, and imaging equipment on four different corn leaf datasets. We further demonstrate that LeafVAE outperforms traditional vegetation indices across multiple applications, including detecting nitrogen deficiency in corn, classifying herbicide stress in soybean, and identifying beech leaf disease using an affordable six-band multispectral camera. 
- Pixel-level explainability, achieved by combining spectral signature composition with interpretable machine learning methods, identifies regions with abnormal spectral characteristics and highlights areas of the leaf that contribute to model predictions. 
- By learning spectral features in an unsupervised manner while still allowing labels for interpretable diagnosis, LeafVAE provides a scalable foundation for automated plant phenotyping across diverse applications.


## Software dependencies
- statsmodels https://www.statsmodels.org/ (Python >=3.9)
- shap https://shap.readthedocs.io/ (Python >=3.9)
- pytorch https://pytorch.org/ (any version should work)
- scipy https://scipy.org/ (any version should work)
- sklearn https://scikit-learn.org/ (any version should work)