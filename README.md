# Fashion-MNIST-Classifier

*By Rohan Mistry - Last updated July 31, 2025*

---

## 📖 Overview

Web application developed using Python and TensorFlow/Keras to classify images of clothing from the Fashion MNIST dataset. Users can upload grayscale 28x28 images of apparel items to receive predictions from several machine learning models including Logistic Regression, KNN, Neural Networks, and CNNs. The app also supports evaluation on the test set with detailed visualizations.

**Target Users** are students, developers, and enthusiasts interested in computer vision, machine learning, and image classification workflows.

🔗 **Try it live**: [fashionmnist-classifier.streamlit.app](https://fashionmnist-classifier.streamlit.app)

<br>

![](/static/img/streamlit_demo_application.png)

---

## 📁 Contents

```bash
├── data/
│   └── data.py          # Dataset loading and preprocessing script
├── models/              # ML model definitions and training logic
├── output/
│   └── visualization.py        # Model performance visualizations
├── saved_models/        # Pre-trained models
├── static/           
│   └── sample_images/   # Sample Fashion MNIST images for testing
├── utils/           
│   └── inference.py     # Utility functions for model inference
├── web/           
│   └── app.py           # Streamlit frontend app
├── LICENSE              # MIT License
├── README.md            # Project documentation
└── requirements.txt     # Python dependencies
```

---

## 🌟 Features

* **Model Selection**: Choose from Logistic Regression, KNN, Neural Network, or CNN models for classification.
* **Image Upload**: Upload your own clothing images in JPG, JPEG, or PNG formats.
* **Live Prediction**: View predicted class and confidence score for uploaded images.
* **Prediction Visualization**: Bar charts display class probabilities for better interpretation.
* **Evaluation Mode**: Evaluate selected model on Fashion MNIST test set with confusion matrix visualization.
* **Preprocessed Samples**: Included sample Fashion MNIST test images and pre-trained models for quick testing.

---

## 🛠️ Installation Instructions

To run the app locally:
1. Clone the repository:
```bash
git clone https://github.com/rmluck/Fashion-MNIST-Classifier.git
cd Fashion-MNIST-Classifier
```
2. Set up a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate
```
3. Install dependencies
```bash
pip install -r requirements.txt
```
4. Launch the app:
```bash
streamlit run web/app.py
```

---

## 💡 Usage

**Step 1: Select Model**

Select desired model from sidebar. Choose between Logistic Regression, KNN, Neural Network, or CNN.

**Step 2: Upload Images**

Upload JPG, JPEG, or PNG images of clothing items to get predictions. Find your own or use the provided [sample images](/static/sample_images/).

**Step 3: View Prediction**:

View model's prediction and confidence score for selected image(s) along with visualization charting probability for each possible label.

![](/static/img/prediction_results.png)

**Step 4: Evaluate Model**:

Run evaluation on the entire Fashion MNIST test set to view confusion matrix and model performance metrics.

![](/static/img/evaluation_metrics.png)

---

## 🚧 Future Improvements

* Add more robust evaluation metrics.
* Add support for batch uploads and batch prediction.
* Provide downloadable prediction reports.
* Add model training interface for user customization.
* Improve UI/UX with dark mode and interactive visualizations.
* Optimize model inference speed with TensorFlow Lite or ONNX.
* Unit test key functions.
* Add image augmentation options to improve model robustness.
* Support mobile-friendly interface.

---

## 🧰 Tech Stack

* Python
* **Frontend**: [Streamlit](https://streamlit.io/)
* **Machine Learning**: TensorFlow/Keras, `scikit-learn`
* **Data Processing**: `numpy`, `PIL` (Pillow)
* **Visualization**: `matplotlib`, `seaborn`, `pandas`
* **Deployment**: Streamlit Community Cloud

## 🙏 Contributions / Acknowledgements

This project was built independently as a portfolio project to demonstrate practical machine learning workflows. Inspired by a course project I did using the Fashion-MNIST dataset.

## 🪪 License

This project is licensed under the [MIT License](/LICENSE).