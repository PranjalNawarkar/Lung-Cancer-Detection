
# Neural Convolutional Networks Finding Cancerous Nodules in Patients' Lungs Using CT Scans

![Stargazers](https://img.shields.io/github/stars/atharva21-stack/LungCancerDetection)
![Issues](https://img.shields.io/github/issues/atharva21-stack/LungCancerDetection)
![Forks](https://img.shields.io/github/forks/atharva21-stack/LungCancerDetection)

## Introduction 👋
Each year, around 225,000 individuals die in the United States as a result of lung cancer, with an additional monetary loss of $12 billion. The Vice President's office devotes special attention to the early detection of lung cancer, as this can boost the victims' chances of survival. In this project we are detecting malignant blobs and nodules in patients' CT scans using a powerful machine learning algorithm. We decided to work on the Data Science Bowl 2017 problem because it was an interesting problem with a wide range of approaches for devising a solution.


## Data & Pre-processing 🔀

- Two categories of data sets provided:
        
        1) Set of images of the CT scans of different patients.
        2) Set of labels for the patients.

#### Note: The number of CT scan images for every patient is not fixed & hence, the number of the images is different.

## Timeline of the tasks
Data provided by the contributors are DICOM files of patients’ CT scan therefore it involves complicated pre-processing methods in order to get into the form that is usable to apply deep learning and machine learning methodologies to it. The following is a timeline of the tasks involved in the preprocessing steps:

### Loading the DICOM files: 
Pixel information for each file, as well as associated metadata, is obtained from each patient's scan and is extremely useful.

### Adding missing metadata: 
The 'z' axis' missing metadata is inferred.

### Converting the pixel values to Hounsfield Units (HU): 
The density of the matter shown in that position in the scan is represented by Hounsfeld Units, which are converted from pixel units.

### 3D plotting: 
Because CT scans are 3D images. Visualizing them in a 3D structure helps us understand what we're looking at.

### Lung Segmentation: 
Lung segmentation is the process of identifying lungs' boundaries in a CT scan image. Thresholding the pixels, setting a specific colour for the air background, and using dilation and erosion operations for better separation and clarity removes lung tissue, blood in the heart, muscles, and other lean tissues.

### Normalization: 
Normalization is a good approach in deep learning, and since this problem involves Hounsfeld Units, the pixel values must be normalized.

### Zero Centering: 
Zero scaling is useful for reducing the effect of scaling differences and relying solely on the content of the images.

## Installation ⏬

* Python (3.11.0)
* pandas (1.5.2)
* PyTorch (1.13.0)
* opencv-python (4.6.0)
* NumPy (1.23.5)
* SciPy (1.6.0)
* H5py (3.7.0)
* torchvision (0.14.0)
* tqdm (4.64.1)
* imageio (2.22.4)

## License 📜
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)


## Contributing ✨

Contributions are always welcome!

See [CONTRIBUTING.md](https://github.com/atharva21-stack/LungCancerDetection/blob/main/CONTRIBUTING.md) for ways to get started.

Please adhere to this project's [CODE-OF-CONDUCT.md](https://github.com/atharva21-stack/LungCancerDetection/blob/main/CODE-OF-CONDUCT.md).





## Authors 👨‍💻

- [PranjalNawarkar]([https://www.github.com/atharva21-stack](https://github.com/PranjalNawarkar))

## Links 🔗
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nawarkarpranjal/)


## Feedback 🙋‍
If you have any feedback, please reach out to me at <a src="mailto:nawarkarpranjal@gmail.com">nawarkarpranjal@gmail.com</a>
