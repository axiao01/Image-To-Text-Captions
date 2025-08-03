# Image-To-Text-Captions

This repository contains the code for an image captioning project trained on the Flickr8k dataset. It uses a pre-trained ResNet-50 as an encoder to extract image features, and provides three decoder options—LSTM, GRU, and Transformer—to generate descriptive captions from image embeddings.

### 1. Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
  
### 2. Clone the Repository
`git clone https://github.com/axiao01/Image-To-Text-Captions.git`

### 3. Install Dependencies
Install all required Python packages using pip:

`pip install -r requirements.txt`

### 4. Navigate to a Decoder Subfolder
This repository provides three different decoder models. Each decoder is implemented in its own subdirectory listed below. To run each choice of decoder, `cd` to the correct sub-folder. For example, `cd LSTM`, `cd Transformer`, or `cd GRU`. Each sub-folder may contain its own `README.md` with specific instructions. If not, the Jupyter Notebook can typically be run directly after installing dependencies.

- `LSTM/` – Image captioning using an LSTM-based decoder

- `GRU/` – Image captioning using a GRU-based decoder

- `Transformer/` – Image captioning using a Transformer-based decoder
