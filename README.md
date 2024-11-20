# Suspicious Link Analyzer 🚨

## Overview
Suspicious links pose a significant cybersecurity threat by exploiting deceptive URLs to trick users into accessing malicious websites or divulging sensitive information. This project aims to mitigate such risks by leveraging **Machine Learning** and **Deep Neural Networks** to detect and classify potentially harmful links. Using a carefully curated dataset of both malicious and benign URLs, we extract critical features to train and evaluate various models for optimal performance.

---

## Objective 🎯
The goal is to analyze and predict malicious URLs by:
1. Extracting essential features from domain, HTML content, and address bars.
2. Training multiple machine learning models to classify URLs as "suspicious" or "legitimate."
3. Evaluating model accuracy and fine-tuning for maximum detection capability.

---

## Features 📋

### 🔍 **Feature Extraction**
- URL attributes such as domain age, HTTPS presence, and anchor tags.
- Webpage-based data, including HTML content and website traffic.
- Address bar attributes like long URLs or presence of suspicious characters.

### 🧠 **Machine Learning Models**
- Gradient Boosting Classifier: Top performer with **97.4% accuracy**.
- CatBoost Classifier, Random Forest, Multi-layer Perceptron, and more.
- Refer to **SuspiciousLinkAnalyzer.ipynb** for detailed performance metrics.

### 📊 **Results**
| ML Model                   | Accuracy | f1_score | Recall | Precision |
|----------------------------|----------|----------|--------|-----------|
| Gradient Boosting Classifier | 0.974    | 0.977    | 0.994  | 0.986     |
| CatBoost Classifier         | 0.972    | 0.975    | 0.994  | 0.989     |
| Multi-layer Perceptron      | 0.969    | 0.973    | 0.995  | 0.981     |

---

## Technologies Used 🛠️
- **Python**: Core development language.
- **Numpy**: Data manipulation.
- **Pandas**: Data handling.
- **Matplotlib**: Visualization.
- **Scikit-learn**: Machine learning models.
- **Flask**: Web integration.

---

## Installation ⚙️
Fork and clone the repository. Install the dependencies:
```bash
pip install -r requirements.txt
```

---

## Web Application 🌐
The system provides an interactive webpage for users to input URLs. It processes the URLs in real-time, extracts features, and predicts the probability of the link being suspicious with a user-friendly interface.

---

## Conclusion ✅
- **Gradient Boosting Classifier** emerged as the most accurate model with **97.4% classification accuracy**, significantly reducing the risks associated with malicious links.
- Features like HTTPS presence, anchor URLs, and website traffic play a crucial role in detecting suspicious links.
- This project serves as a hands-on exploration of data preprocessing, feature engineering, and model optimization.

---

## Future Enhancements 🔮
1. Real-time detection integration.
2. Feature improvement through advanced natural language processing.
3. Extension to detect malicious attachments and embedded threats.

---

Feel free to contribute, report issues, or suggest enhancements! 🚀
```
