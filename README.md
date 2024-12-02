BY- 	MOhammed Fahad Altamash-211IT041
 Kunal Tomar - 211IT035

# Medical Image Reporting using Attention Mechanism

This project implements an attention-based model for generating textual reports from medical images (X-rays). The model uses CheXNet as a backbone for image feature extraction and a custom attention-based encoder-decoder architecture for report generation.

## Features

- **CheXNet Backbone**: Pre-trained DenseNet-121 model for feature extraction from medical images.
- **Attention Mechanism**: Global attention layer integrated into the decoder to focus on relevant parts of the images.
- **Dual Image Input**: Supports two images for feature concatenation and improved context understanding.
- **Greedy Search Prediction**: Generates textual reports using a greedy decoding algorithm.

## Prerequisites

Ensure the following packages are installed:
- Python 3.x
- TensorFlow 2.x
- OpenCV
- NLTK
- Joblib
- Pandas
- NumPy

Install missing dependencies using:
```bash
pip install tensorflow opencv-python nltk joblib pandas numpy
/content/drive/My Drive/Medical image Reporting/
│
├── Images/                  # Folder containing input medical images
├── pickle_files/            # Folder containing preprocessed data files
│   ├── train.pkl            # Training data pickle file
│   ├── test.pkl             # Testing data pickle file
├── ChexNet weights/         # Folder containing pre-trained CheXNet weights
│   ├── brucechou1983_CheXNet_Keras_0.3.0_weights.h5
├── tokenizer.pkl            # Tokenizer for text preprocessing
└── Encoder_Decoder_global_attention.h5  # Pre-trained model weights
