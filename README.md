![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)

# LeafVAE

**Variational autoencoder enables unsupervised leaf diagnosis via hyperspectral imaging**

LeafVAE is a variational autoencoder framework that learns spectral signatures directly from hyperspectral leaf images without manual annotation. Our model encodes leaf spectra into a compact, two-dimensional latent space where pixels cluster by spectral similarity, creating quantitative leaf descriptors from signature composition that facilitate downstream phenotyping tasks. <br />
We found that the learned representations generalize robustly across genotypes, years, and imaging equipment on four different corn leaf datasets. We further demonstrate that LeafVAE outperforms traditional vegetation indices across multiple applications, including detecting nitrogen deficiency in corn, classifying herbicide stress in soybean, and identifying beech leaf disease using an affordable six-band multispectral camera. 

## Approach

![alt text](https://github.com/Kangyu-Ji/LeafVAE/blob/main/Figure/Fig1.png?raw=true)

## Software dependencies
- statsmodels https://www.statsmodels.org/ (Python >=3.9)
- shap https://shap.readthedocs.io/ (Python >=3.9)
- pytorch https://pytorch.org/ (any version should work)
- scipy https://scipy.org/ (any version should work)
- sklearn https://scikit-learn.org/ (any version should work)

## Explainability
Pixel-level explainability, achieved by combining spectral signature composition with interpretable machine learning methods, identifies regions with abnormal spectral characteristics and highlights areas of the leaf that contribute to model predictions. 
![alt text](https://github.com/Kangyu-Ji/LeafVAE/blob/main/Figure/Fig2.png?raw=true)


## About us
- ABE Plant Sensor Lab @Purdue https://engineering.purdue.edu/ABEPlantSensorLab