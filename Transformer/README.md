# Image-To-Text-Captions

This repository contains the code for an image captioning model trained on the Flickr8k dataset. The model uses a pre-trained ResNet-50 as an encoder to extract image features and different choices of models as a decoder to generate descriptive captions.

### 1. Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
  
### 2. Clone the Repository
`git clone https://github.com/axiao01/Image-To-Text-Captions.git`

### 3. Install Dependencies
Install all required Python packages using pip:

`pip install -r requirements.txt`

### 4. Download the Flickr8k Dataset (Required for Transformer Notebook)

The Flickr8k dataset is required to run this notebook. It is available on [Kaggle](https://www.kaggle.com/datasets/adityajn105/flickr8k?resource=download).

Navigate to the Flickr8k Dataset page on Kaggle.

Download the dataset zip file.

Unzip the contents into the project directory, ensuring the following structure:

````
your_project_folder/
├── Img2Text_Final_Optimized.ipynb
├── archive/
│   ├── Images/                 (This folder contains all the input images)
│   │   ├── image1.jpg
│   │   ├── image2.jpg
│   │   └── ...
│   └── captions.txt           (This file contains image-caption pairs)
├── TestPic/                   (Optional: contains custom images for inference)
│   ├── example1.png
│   └── ...
├── requirements.txt
└── (other folders for outputs such as models/, logs/, cached_features/, etc.)
````

### 5. Running the Notebook (Transformer)
Start Jupyter Notebook or JupyterLab from the project directory:

Open the Img2Text_Final_Optimized.ipynb notebook.

Run all the cells in order. The notebook will automatically:

- Download necessary NLTK data.

- Build a custom vocabulary from image captions.

- Apply data augmentation and load the Flickr dataset.

- Extract image features using a pre-trained ResNet-50 model.

- Train a Transformer Decoder model for caption generation.

- Generate captions for sample images.

- Evaluate results using BLEU score.

You can customize training parameters in the Setup and Configuration section.

