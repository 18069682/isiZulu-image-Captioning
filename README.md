## COS 801 Project – Bridging the Visual-Linguistic Divide An Automated Image Captioning System for isiZulu using Deep Visual Attention Models

## Project Overview
This project implements an image captioning system that generates isiZulu descriptions for images using deep learning models with visual attention. The system leverages the Flickr8k dataset and integrates custom isiZulu captions for linguistic diversity.

# Steps to Run the Project


** Step 1: Open the Notebook in Google Colab
Upload isizulu_captioning.ipynb to Google Colab.

**Step 2: Upload isiZulu Captions File
Upload zu_captions.json to /content/ in Colab.

**Step 3: Run All Cells in the Notebook
The notebook will:

Install required packages (torch, torchvision, nltk, pillow, etc.)
Download and extract the Flickr8k dataset
Load English and isiZulu captions
Validate image-caption alignment
Display sample images with captions

** Step 4: HuggingFace Token (If Prompted in cell 9)
Some versions of the pipeline require HuggingFace authentication for translation models.
Use:
Name: HF_TOKEN  
Value: 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 Paste this token when prompted and rerun the cell.

Step 5: Train the Model

Train the encoder-decoder model
Evaluate BLEU score and accuracy
Save checkpoints under /content/models/

Link to datasets:
Kaggle flickr8 dataset: https://www.kaggle.com/datasets/adityajn105/flickr8k
GitHub flickr8 dataset: https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_Dataset.zip
