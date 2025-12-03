COS 801 Project – Bridging the Visual-Linguistic Divide
An Automated Image Captioning System for isiZulu using Deep Visual Attention Models

Project Overview
This project implements an image captioning system that generates isiZulu descriptions for images using deep learning models with visual attention. The system leverages the Flickr8k dataset and integrates custom isiZulu captions for linguistic diversity.

Repository Structure
.
├── isizulu_captioning.ipynb   # Main notebook
├── zu_captions.json           # isiZulu captions mapping
├── results/                   # Output samples and evaluation
└── README.md                  # Project documentation


Requirements


Files Needed

isizulu_captioning.ipynb
zu_captions.json



Dependencies

Installed automatically in the notebook:
torch, torchvision, nltk, pillow, etc.




How to Run


Open the Notebook in Google Colab

Upload isizulu_captioning.ipynb to Colab.

Upload isiZulu Captions

Upload zu_captions.json to /content/.

Run All Cells

The notebook will:

Install dependencies
Download Flickr8k dataset
Load English and isiZulu captions
Validate image-caption alignment
Display sample images with captions

Optional: Train the Model

Train the encoder-decoder model
Evaluate BLEU score and accuracy
Save checkpoints under /content/models/




File Details


isizulu_captioning.ipynb

Data loading and preprocessing
Caption alignment checks
Visualisation utilities
Model training and evaluation (optional)



zu_captions.json

Dictionary mapping image filenames to isiZulu captions:
JSON{  "1000268201_693b08cb0e.jpg": ["Umfana ugxuma esihlalweni"],  "1001773457_577c3a7d70.jpg": ["Indoda igibela isithuthuthu"]}Show more lines

Outputs

Sample aligned captions
Train/test splits
Random image-caption visualisations
If training is enabled:

Loss curves
BLEU scores
Predicted captions for test images




Dataset
We use the https://www.kaggle.com/datasets/adityajn105/flickr8k, originally annotated in English. Captions were translated into isiZulu and verified for accuracy.
Download Instructions:

Sign in to https://www.kaggle.com/.
Download the dataset from https://www.kaggle.com/datasets/adityajn105/flickr8k.
Extract and place it inside the data/ folder.
