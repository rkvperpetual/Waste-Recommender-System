
# ♻️ AI-Based Waste Recommender System

This project implements an AI-powered waste classification and recommendation system designed to promote sustainable waste management practices. By leveraging machine learning techniques, the system classifies waste items and provides users with guidance on reuse and recycling options.

## 🚀 Features

- **Waste Classification**: Utilizes machine learning algorithms to classify waste into categories such as plastic, metal, glass, paper, and organic waste.
- **Reuse and Recycle Recommendations**: Offers suggestions for reusing or recycling classified waste items, encouraging eco-friendly practices.
- **User-Friendly Interface**: Provides a web-based interface for users to upload images of waste items and receive instant classification and recommendations.
- **Data Visualization**: Includes visual representations of waste categories and recycling statistics to raise awareness.

## 🗂️ Project Structure

```
Waste-Recommender-System/
├── app.py                      # Flask web application
├── model.ipynb                 # Jupyter Notebook for model training
├── model2.ipynb                # Alternative model training notebook
├── scrapper.py                 # Script for data scraping
├── kmeans_clusters.npy         # Saved KMeans clustering model
├── pca_features.npy            # PCA features for dimensionality reduction
├── requirements.txt            # Python dependencies
├── templates/
│   └── index.html              # HTML template for the web interface
├── static/
│   └── styles.css              # CSS styles for the web interface
├── uploads/                    # Directory for storing uploaded images
└── data/                       # Directory containing dataset files
```

## 📊 Dataset

The system is trained on a dataset comprising various waste items categorized into recyclable and non-recyclable classes. The dataset includes images and corresponding labels, facilitating supervised learning for waste classification.

## 🧠 Model Training

- **Preprocessing**: Images are resized, normalized, and augmented to enhance model robustness.
- **Feature Extraction**: Principal Component Analysis (PCA) is applied to reduce dimensionality and extract significant features.
- **Clustering**: KMeans clustering is employed to group similar waste items, aiding in classification.
- **Model Saving**: Trained models and features are saved as `.npy` files for deployment.

## 🧪 Installation and Usage

1. **Clone the Repository**

   ```bash
   git clone https://github.com/rkvperpetual/Waste-Recommender-System.git
   cd Waste-Recommender-System
   ```

2. **Create a Virtual Environment (Optional but Recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Flask Application**

   ```bash
   python app.py
   ```

5. **Access the Web Interface**

   Open your web browser and navigate to `http://127.0.0.1:5000/` to use the waste recommender system.

## 📌 Dependencies

- Python 3.x
- Flask
- pandas
- scikit-learn
- numpy
- matplotlib
- seaborn
- OpenCV
- Jupyter Notebook

Ensure all dependencies are installed by running:

```bash
pip install -r requirements.txt
```

## 🤝 Contributing

Contributions are welcome! If you'd like to enhance this project:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request detailing your changes.

## 📄 License

This project is licensed under the [MIT License](LICENSE).
