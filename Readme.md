# 🧠 Dog Breed Identification – Model Training

This repository contains the full code and resources used to train a deep learning model for identifying dog breeds from images using transfer learning (MobileNetV2). The model was trained on the [Kaggle Dog Breed Identification dataset](https://www.kaggle.com/c/dog-breed-identification) and achieves over 90% accuracy.

## 🐶 Dataset

- **Source**: [Kaggle - Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification)
- **Images**: 20,000+ (Train: 10,000+ | Test: 10,000+)
- **Breeds**: 120

> 💡 Download the dataset from Kaggle and extract it into the `data/` directory.

## 🔍 Model Details

- **Architecture**: MobileNetV2 (pre-trained on ImageNet)
- **Input Shape**: 224x224x3
- **Loss Function**: Categorical Crossentropy
- **Optimizer**: Adam
- **Metrics**: Accuracy
- **Techniques Used**:
  - Transfer Learning
  - Fine-tuning Top Layers
  - EarlyStopping Callback
  - TensorBoard Logging

## 🧪 Training

You can run the training either via the Jupyter notebook or the script.

### Option 1: Run in Jupyter Notebook

```bash
cd notebooks/
jupyter notebook training.ipynb
```

### Option 2: Run as Script

```bash
python utils/trainer.py
```

After training, the model will be saved as `models/dog_breed_model.h5`.

## 🛠️ Setup Instructions

1. Clone the repository

   ```bash
   git clone https://github.com/Sumit-72/Dog-Vision
   cd Dog-Vision-Training
   ```

2. Create a virtual environment and activate it (optional)

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```

4. Download and extract the dataset from Kaggle into the `data/` folder.

5. Start training (via notebook or script)

## 📦 Export Trained Model

To export the model in `.h5` format for deployment:

```bash
python export_model.py
```

This will save the model in the `models/` directory.

## 🧾 Requirements

- Python 3.11
- TensorFlow 2.15.0
- NumPy 1.25.2
- Pandas

(See `requirements.txt` for the full list)

## 📌 Related Repos

- 🖥️ **Web App Deployment**: [Dog-Vision Streamlit App](https://github.com/Sumit-72/Dog_vision_web)
- 🔗 **Live App**: [Try the live demo](https://dog-vision72.streamlit.app/)

## Author

**Sumit Shekhar**  
[GitHub](https://github.com/Sumit-72) | [LinkedIn](https://www.linkedin.com/in/sumit-shekhar72)