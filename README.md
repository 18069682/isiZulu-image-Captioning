# 📊  COS 801 – Project Report 2025-Bridging the Visual-Linguistic Divide: An Automated Image Captioning System for isiZulu using Deep Visual Attention Models

![Made with Python](https://img.shields.io/badge/Made%20with-Python-blue?logo=python)
![Big Data](https://img.shields.io/badge/Focus-Big%20Data-orange)
![Status](https://img.shields.io/badge/Assignment-Completed-brightgreen)




📁 Repository Structure
.
├── isizulu_captioning.ipynb     # Main notebook with dataset prep and caption alignment
├── zu_captions.json             # isiZulu captions file (provided separately)
├── README.md                    
└── results/                     # Evaluation outputs, sample captions, model results

🔧 Requirements

You only need the following files:

isizulu_captioning.ipynb

zu_captions.json
⚠️ If the Notebook Asks for an HF Token (Cell 9)

Some versions of the pipeline require HuggingFace authentication to load translation models.

If prompted for a token:

Name: HF_TOKEN
Value: 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


Paste this into the input box and run the cell again.
All Python dependencies (torch, torchvision, nltk, pillow, etc.) are installed automatically inside the notebook.

🚀 How to Run the Project (Step-by-Step)
1️⃣ Open the Notebook in Google Colab

Click:
File → Upload notebook → Select isizulu_captioning.ipynb

2️⃣ Upload the isiZulu Captions File

In Colab:

Click the Files icon on the left

Click Upload

Upload zu_captions.json

Ensure it appears at:

/content/zu_captions.json

3️⃣ Run the Notebook Cells Top-to-Bottom

The notebook will automatically:

✔ Install needed packages
✔ Create folder structure
✔ Download Flickr8k dataset
✔ Extract all images
✔ Load & clean English captions
✔ Load isiZulu captions from JSON
✔ Validate caption–image alignment
✔ Display sample images + captions

You should see a printed message like:

Successfully loaded 4040 isiZulu captions!

4️⃣ Model Training (Optional Section)

If your version includes model training:

Train the encoder-decoder model

Evaluate BLEU & accuracy

Save checkpoints under /content/models/

📝 File Details
isizulu_captioning.ipynb

Includes:

Imports & installs

Dataset downloader for Flickr8k

Caption preprocessing

JSON loader for isiZulu captions

Image-caption pairing validation

Visualization utilities

zu_captions.json

Custom dictionary mapping:

{
  "1000268201_693b08cb0e.jpg": ["Umfana ugxuma esihlalweni"],
  "1001773457_577c3a7d70.jpg": ["Indoda igibela isithuthuthu"],
  ...
}

📊 Outputs

The notebook generates:

Sample aligned captions

Train/test split tables

Random sample image–caption displays

Translation and captioning quality checks

If training is included:

Model loss curve

BLEU scores

Predicted captions for test images

We use the [Flickr8k dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k), originally annotated in English.  
For this project, captions are translated into isiZulu with human verification to ensure linguistic accuracy.  

### Download Instructions
1. Sign in to [Kaggle](https://www.kaggle.com/).
2. Go to the [dataset link](https://www.kaggle.com/datasets/adityajn105/flickr8k).
3. Download and extract the dataset.
4. Place it inside the `data/` folder of this repository:





