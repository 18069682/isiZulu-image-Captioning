📊 COS 801 – isiZulu-image-Captioning
Made with Python Big Data Status Accuracy


📊 Dataset Information
Images: 8,000 Flickr images (subset of 50% for training)


We use the [Flickr8k dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k), originally annotated in English.  
For this project, captions are translated into isiZulu with human verification to ensure linguistic accuracy.  

### Download Instructions
1. Sign in to [Kaggle](https://www.kaggle.com/).
2. Go to the [dataset link](https://www.kaggle.com/datasets/adityajn105/flickr8k).
3. Download and extract the dataset.
4. Place it inside the `data/` folder of this repository:

Captions per image: 5 each in English and isiZulu

Split:

Training: 50% of original training set (~3,000 images)

Testing: Full test set (~1,000 images)

🎯 Expected Output
After running all cells successfully, you should see:

✅ All packages installed

✅ Folder structure created

✅ Dataset downloaded and extracted

✅ 3 sample images displayed with English captions

✅ isiZulu captions loaded with statistics:

text
Train images: X
Test images: Y
Images with Zulu captions: Z
💾 Saving Your Work
To save your work after running:

Save the notebook: File → Save

Download files: Select files in file browser → Download

Save to Google Drive (optional):

python
from google.colab import drive
drive.mount('/content/drive')
# Then copy files to your Drive
📞 Support
If you encounter any issues:

Check the error message in Colab


IsiZulu Image Captioning Project
📖 Description
A deep learning project that generates isiZulu captions for images using the Flickr8k dataset. The model combines computer vision (ResNet-50) with natural language processing (LSTM) to create descriptive captions in isiZulu.

🚀 Quick Start (Google Colab)
Prerequisites
Google account

Access to Google Colab

Step-by-Step Setup
Upload Files to Colab

Open Google Colab

Upload isizulu_captioning.ipynb (the main notebook)

Upload zu_captions.json (the isiZulu translations)

Run the Notebook
Execute cells in order:

python
# Cell 1: Install dependencies
# Cell 2: Create directory structure
# Cell 3: Download Flickr8k dataset
# Cell 4: Create dataset subset (50% training)
# Cell 5: Visualize sample images
# Cell 6: Load isiZulu captions from JSON
Verify File Locations
Ensure files are in these paths:

text
/content/isizulu_image_captioning/    # Auto-created
/content/zu_captions.json             # Your uploaded file
📁 Project Structure
text
isizulu_image_captioning/
├── data/
│   ├── images/Flickr8k_images/          # Downloaded images
│   └── captions/
│       ├── en/                          # English captions
│       └── zu/                          # isiZulu captions (from JSON)
├── logs/                                # Training logs
├── results/                             # Generated captions
└── tokenizer/                           # SentencePiece model
📊 Dataset Details
Source: Flickr8k dataset (8,000 images)

Captions: 5 per image in both English and isiZulu

Split: 50% training (~3,000 images) + full test set (~1,000 images)

Translation: Machine-translated with human validation

🔧 Installation & Dependencies
Core Requirements
bash
# Main packages
torch>=1.9.0
torchvision>=0.10.0
transformers>=4.12.0
sentencepiece>=0.1.96
sacrebleu>=2.0.0

# Data handling
datasets>=1.18.0
pandas>=1.3.0
numpy>=1.21.0

# Visualization
matplotlib>=3.4.0
Pillow>=8.3.0
Quick Install
python
!pip install torch torchvision transformers sentencepiece
!pip install datasets pandas matplotlib Pillow
🏃‍♂️ Running the Model
1. Data Preparation
python
# Load isiZulu captions
with open('/content/zu_captions.json', 'r') as f:
    zu_captions = json.load(f)
2. Model Components
Encoder: ResNet-50 (pretrained on ImageNet)

Decoder: LSTM with attention mechanism

Tokenizer: SentencePiece for isiZulu

3. Training
python
# Example training call
model.train(
    epochs=20,
    batch_size=32,
    learning_rate=1e-4
)
📈 Expected Output
Successful execution shows:

✅ Package installation confirmation

📁 Directory structure creation

⬇️ Dataset download progress

🖼️ Sample images with captions

📊 Dataset statistics:

text
Train images: 3,040
Test images: 1,000
Available isiZulu captions: 4,040



