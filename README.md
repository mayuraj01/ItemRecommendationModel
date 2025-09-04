# 👗 Fashion Recommendation System

This project is an **AI-powered Fashion Recommender** built with **TensorFlow, Scikit-learn, and Streamlit**.  
It suggests visually similar fashion items when you upload a product image.

---

## 🚀 Features
- Extracts image embeddings using **ResNet50 (ImageNet pretrained)**.
- Stores extracted features for fast similarity search.
- Uses **K-Nearest Neighbors (KNN)** with **cosine similarity** for recommendations.
- Simple **Streamlit UI** to upload an image and view recommended items.
- Easily extendable with other models like **EfficientNet, MobileNet, or VGG16** for better accuracy.

---

## 📂 Project Structure
      ├── images/ # Dataset of product images
      ├── upload/ # Uploaded images via Streamlit
      ├── recom-model.py # Feature extraction & feature dump script
      ├── app.py # Streamlit app for recommendations
      ├── Images_features.pkl # Pickled feature embeddings (generated)
      ├── filesnames.pkl # Pickled list of image filenames
      └── README.md # Project documentation

## Create a virtual environment:
        python -m venv venv
        source venv/bin/activate  # On Linux/Mac
        venv\Scripts\activate     # On Windows

## 📦 Dependencies
Python,
TensorFlow,
NumPy,
Scikit-learn,
Streamlit,
Pillow

Install via:
  - pip install tensorflow numpy scikit-learn streamlit pillow

## 🛠 Usage
Step 1: Extract Features

Run the following to generate embeddings:
python recom-model.py


This will create:
- Images_features.pkl
- filesnames.pkl

Step 2: Run the Streamlit App
streamlit run app.py

Step 3: Upload an Image
Upload any fashion image (e.g., dress, shirt, shoes).

The system will display top 5 most similar images from the dataset.

Future Improvements:
- Use EfficientNet / MobileNet for better embeddings.
- Integrate DeepFashion Dataset for fine-tuning.
- Add user personalization (style-based recommendations).

