# Image-To-Text-Captions

This repository contains the code for an image captioning model trained on the Flickr8k dataset. The model uses a pre-trained ResNet-50 as an encoder to extract image features and different choices of models as a decoder to generate descriptive captions.

### 1. Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
  
### 2. Clone the Repository
`git clone https://github.com/axiao01/Image-To-Text-Captions.git`

### 3. Go to the desired sub-folder for each different decoders
Since this repository contains three different choices of decoder models, the project files for each different one is in its corresponding sub-folder. To run each choice of decoder, `cd` to the correct sub-folder. For example, `cd LSTM`. Each sub-folder contains its own  `requirements.txt` and `README.md` necessary for the sub-project.