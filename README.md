<h1 align="center">🌾 Rice-Grain Classifier</h1>
<p align='center'>Implementation of a pre-trained CNN on classification of rice-grain images</p>

## Background
There are various varieties of rice-crop, each variety having it's own distinctive characterstic features of the shape and size of the grain. \
Taking advantage of this variability, this mini-project aims to classify 5 different types of rice-grain based upon their visual features.

### 📚 Dataset
For this particular purpose, the dataset was obtained from the following <a href=https://www.muratkoklu.com/datasets/vtdhnd09.php>resource</a>
The dataset had 5 classes:
<ol>
  <li>Arborio</li>
  <li>Basmati</li>
  <li>Ipsala</li>
  <li>Jasmine</li>
  <li>Karacadag</li>
</ol>
The dataset was balanced with 15k images for each class.

⭐ ***A customised data-augmentation pipline was implemented in code, to increase the variability of the exisiting dataset.***

### 🏗️ Model Architecture
For this particular task, using transfer-learning a pre-trained version of ***MobileNet-v2*** was used, with an input dimension of (160,160,3). \
The top two layers of the model was unfreezed and was allowed to train on the dataset.


