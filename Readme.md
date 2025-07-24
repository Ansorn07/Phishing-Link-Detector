# Phishing Link Detector 🎣

A robust machine learning application built to combat phishing attacks by analyzing and classifying URLs with high accuracy.

## Description

This repository contains the source code for Phishing-Link-Detector, a system designed to identify malicious URLs. It uses comprehensive feature extraction from URLs and a trained classification model to predict whether a link is a phishing attempt, helping to ensure web safety.

-----

## 🚀 Key Features

  * **Advanced Feature Extraction:** Extracts over 30 distinct features from URLs to identify suspicious patterns indicative of phishing.
  * **Pre-Trained ML Model:** Utilizes a highly accurate, pre-trained classifier (`phishing_classifier.pkl`) for real-time predictions.
  * **Comprehensive Dataset Tools:** Includes scripts for generating and processing datasets, allowing for easy retraining and testing.
  * **Detailed Analysis:** Comes with a Jupyter Notebook (`new_training_after_data_generalization.ipynb`) that details the model training, evaluation, and data generalization process.

-----

## 🤔 How It Works

The detection process is straightforward yet powerful:

1.  **Input URL:** A user provides a URL for analysis.
2.  **Feature Extraction:** The system extracts a wide range of features from the URL. This includes analyzing the domain, path, special characters, and length.
3.  **Prediction:** The extracted features are fed into the pre-trained machine learning model.
4.  **Classification:** The model classifies the URL as either **Legitimate** or a **Phishing** attempt.

-----

## 📋 Examples

Here are some examples of how the detector classifies different types of links:

### 🎣 Phishing Links

These links often impersonate legitimate websites to steal sensitive information.

| URL                                                | Prediction |
| -------------------------------------------------- | :--------: |
| `http://paypal.com.login.verify-user.abcxyz.ru/login` | **Phishing** |
| `http://update-your-bank-info.security-alert.net/` | **Phishing** |
| `http://secure-account.amazon.verify-user-check.in/` | **Phishing** |
| `http://apple.com.verify-id-urgent-reset.ga/login`   | **Phishing** |
| `http://facebook.com-security-check-2348.tk/update`  | **Phishing** |

### ✅ Legitimate Links

These are examples of safe, well-known websites.

| URL                                                | Prediction  |
| -------------------------------------------------- | :---------: |
| `https://www.google.com`                           | **Legitimate** |
| `https://www.amazon.in`                            | **Legitimate** |
| `https://www.wikipedia.org`                        | **Legitimate** |
| `https://www.india.gov.in`                         | **Legitimate** |
| `https://www.rbi.org.in`                           | **Legitimate** |

-----

## 🛠️ Installation

To get a local copy up and running, follow these simple steps.

1.  **Clone the repo**
    ```sh
    git clone https://github.com/your_username/Phishing-Link-Detector.git
    ```
2.  **Navigate to the project directory**
    ```sh
    cd Phishing-Link-Detector
    ```
3.  **Install the required packages**
    ```sh
    pip install -r requirements.txt
    ```
    *(Note: You may need to create a `requirements.txt` file based on the libraries used in your scripts, such as pandas, scikit-learn, etc.)*

-----

## Usage

You can use the `app.py` file to run the detector.

```sh
python app.py
```

Follow the on-screen prompts to enter a URL and receive a prediction.

-----

## 🧠 Model

The core of this project is the pre-trained classification model stored in `phishing_classifier.pkl`. This model was trained on a diverse dataset of phishing and legitimate URLs and can be easily loaded for predictions.

For details on the training process, please see the `new_training_after_data_generalization.ipynb` notebook.

-----

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

-----

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
