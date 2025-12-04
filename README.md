![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)

# LeafVAE

**[Paper] Learning the spectral language of leaves for plant health diagnosis**

LeafVAE is a variational autoencoder framework that learns spectral characteristics (subtle color differences) directly from hyperspectral leaf images without manual annotation. 

## Approach

- The model learns spectral signatures of various types of leaves by encoding each leaf spectrum, obtained from a spatial pixel in a hyperspectral image, into a compact 2D latent embedding, from which the decoder reconstructs the original spectrum.
- Thus, all pixels in the dataset can be encoded and projected into a common latent space, where they cluster according to spectral similarity. Each leaf can then be represented as a distribution of cluster compositions, the proportions of different spectral signatures (i.e., colors) within the leaf, which provide a simple and interpretable descriptor of leaf condition. 

![alt text](https://github.com/Kangyu-Ji/LeafVAE/blob/main/Figure/Fig1.png?raw=true)

## Software dependencies
- statsmodels https://www.statsmodels.org/ (Python >=3.9)
- shap https://shap.readthedocs.io/ (Python >=3.9)
- pytorch https://pytorch.org/ (any version should work)
- scipy https://scipy.org/ (any version should work)
- sklearn https://scikit-learn.org/ (any version should work)

## Usage
- Install the dependencies
- Download the [demo dataset](https://purdue0-my.sharepoint.com/:u:/g/personal/ji275_purdue_edu/EesUuxR-2SZFobHFWZDcTFkB92WZzoFFmMiRDj2U3DZuRA?e=LG2IR7) to "Dataset/2022 Corn R1" folder
- Run the jupyter notebook LeafVAE.ipynb

## Explainability
The combination of spectral-signature clustering and Shapley-based feature explanations can show which parts of the leaf have unusual spectral patterns and reveal which areas most influence the model’s predictions.
![alt text](https://github.com/Kangyu-Ji/LeafVAE/blob/main/Figure/Fig2.png?raw=true)


## About us
- Dr. Kangyu Ji https://scholar.google.com/citations?user=Oej20eMAAAAJ
- Prof. Jian Jin https://scholar.google.com/citations?user=rt8TzCkAAAAJ
- ABE Plant Sensor Lab @Purdue https://engineering.purdue.edu/ABEPlantSensorLab