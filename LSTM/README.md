# Image-To-Text-Captions

This repository contains the code for an image captioning model trained on the Flickr8k dataset. This sub folder uses LSTM for decoder.

### Download the Flickr8k Dataset (Optional)

The Flickr8k dataset is required to run this notebook. It is available on [Kaggle](https://www.kaggle.com/datasets/adityajn105/flickr8k?resource=download).

The notebook will automatically download the dataset. After a successful download, your project structure would be like the structure shown below.
You can also manually dowload the dataset from Kaggle and unzip it into this structure.

````
your_project_folder/
├── img2text_lstm_Xiao.ipynb
├── archive/
│   ├── Images/  (This folder contains all the images)
│   │   ├── image1.jpg
│   │   ├── image2.jpg
│   │   └── ...
│   └── captions.txt  (This file contains all the captions)
├── requirements.txt
├── tests/                  (This folder contains test images not in the flikr8k dataset that you can use for displaying)
│   ├──img01.png
│   ├──img02.png
│   └── ...
└── (other folders like cached_features, models will be created here)
````

### Running the Notebook (LSTM)
Start Jupyter Notebook or JupyterLab from the project directory:

`jupyter notebook`

Open the img2text_lstm_Xiao.ipynb notebook.

Run all the cells in order. The notebook will automatically:

- Download necessary NLTK data and dataset.

- Build the vocabulary.

- Pre-extract and cache image features using a pre-trained ResNet-50.

- Train the Encoder-Decoder model.

- Generate a caption for a sample image.

- You can change the training parameters in the Setup and Configureation section
