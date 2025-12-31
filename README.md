# 📰 Fake News Detector

This project uses Deep Learning (Natural Language Processing) to identify whether a news article is real or fake. It features a Bidirectional LSTM model built with Keras and a user-friendly web interface.

## 🚀 Overview
Misinformation is a significant challenge in the digital age. This project aims to automate the detection of "fake news" by analyzing the linguistic patterns of articles. The model was trained on a balanced dataset of real and fake news, achieving a high level of accuracy.

### Key Features
*   **Text Preprocessing:** Automated cleaning (lowercase, punctuation removal, etc.).
*   **Deep Learning:** Utilizes a Bidirectional Long Short-Term Memory (LSTM) network to capture contextual information from text.
*   **Interactive UI:** A real-time web app built with Streamlit (or Gradio) for easy testing.

## 🏗️ Model Architecture
The model is a Sequential neural network with the following layers:

*   **Embedding Layer:** Converts words into 16-dimensional dense vectors.
*   **Bidirectional LSTM:** Processes sequences forward and backward to understand context.
*   **Dense Layers:** Fully connected layers with ReLU activation for feature extraction.
*   **Output Layer:** A single neuron with Sigmoid activation to output a probability (0 to 1).

## 🛠️ Installation & Setup

1.  **Clone the repository**
    ```bash
    git clone https://github.com/Pranav-7890/Fake_News_Detection.git
    cd fake-news-detector
    ```

2.  **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```
## 📝 Requirements.txt

This file tells the server (like Hugging Face) exactly which libraries to install. Keep it simple to avoid version conflicts.
```bash
### Required Libraries
numpy
pandas
matplotlib
seaborn
tensorflow
sklearn
nltk
re
pickle
```


### Required Files
Ensure you have the following files in the project root:
*   `fake_news_detector.keras` (Trained model)
*   `tokenizer.pickle` (Saved word index)

## 💻 Usage

### Running Locally
To launch the web interface on your local machine:
```bash
streamlit run app.py
```

### In the Jupyter Notebook
Open `fake_news.ipynb` to see the full training process, including:
*   Data Exploration (EDA)
*   Text cleaning and Tokenization
*   Model training and Validation
*   Performance metrics (Accuracy/Loss curves)

## 📊 Results

| Metric | Value |
| :--- | :--- |
| **Training Accuracy** | ~91% |
| **Validation Accuracy** | ~89% |

> **Note:** The model performs best on full-text news articles rather than short headlines.

## 📁 Project Structure

```plaintext
├── .venv/                   # Virtual environment
├── app.py                   # Streamlit web application
├── fake_news.ipynb # Training & Analysis notebook
├── fake_news_detector.keras    # Saved Keras model
├── tokenizer.pickle         # Tokenizer object for preprocessing
└── requirements.txt         # List of dependencies
```

## 👤 Author
**Your Name** - [GitHub](https://github.com/Pranav-7890) | [LinkedIn](https://www.linkedin.com/in/pranav-kumar-g/)
