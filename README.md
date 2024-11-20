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
The following machine learning models were tested, and their performances were compared based on key metrics:
| Model                     | Accuracy | f1_score | Recall | Precision |
|---------------------------|----------|----------|--------|-----------|
| Gradient Boosting Classifier | 0.974    | 0.977    | 0.994  | 0.986     |
| CatBoost Classifier         | 0.972    | 0.975    | 0.994  | 0.989     |
| Multi-layer Perceptron      | 0.969    | 0.973    | 0.995  | 0.981     |
| Random Forest               | 0.967    | 0.971    | 0.993  | 0.990     |
| Support Vector Machine      | 0.964    | 0.968    | 0.980  | 0.965     |
| Decision Tree               | 0.960    | 0.964    | 0.991  | 0.993     |
| K-Nearest Neighbors         | 0.956    | 0.961    | 0.991  | 0.989     |
| Logistic Regression         | 0.934    | 0.941    | 0.943  | 0.927     |
| Naive Bayes Classifier      | 0.605    | 0.454    | 0.292  | 0.997     |

The **Gradient Boosting Classifier** achieved the highest accuracy, making it the most suitable for this task.

---

## Technologies Used 🛠️
- **Python**: Core development language.
- **Numpy**: Data manipulation.
- **Pandas**: Data handling.
- **Matplotlib**: Visualization.
- **Scikit-learn**: Machine learning models.
- **Flask**: Web application development.

---

## Installation ⚙️
To set up the project locally, follow these steps:

1. Fork and clone the repository.
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Web Application 🌐
The system includes an interactive web application where users can input URLs for analysis. The application:
- Extracts features from the given URL.
- Predicts the probability of the URL being suspicious or legitimate.
- Displays the results in a user-friendly format.

The app is built using **Flask** and can be extended for real-time monitoring and integration into larger systems.

---

## Dataset 📂
The dataset comprises both phishing and legitimate URLs. Key features extracted include:
- Presence of HTTPS.
- URL length and domain age.
- Anchor tags and website traffic data.

The dataset is preprocessed to enhance the performance of machine learning models. More details are available in the `SuspiciousLinkAnalyzer.ipynb` file.

---

## Results 📊
| **Metric**                 | **Best Model (Gradient Boosting)** |
|----------------------------|-------------------------------------|
| Accuracy                   | 0.974                              |
| f1_score                   | 0.977                              |
| Recall                     | 0.994                              |
| Precision                  | 0.986                              |

The **Gradient Boosting Classifier** significantly outperformed other models, achieving a near-perfect accuracy rate and excellent precision-recall balance.

---

## Conclusion ✅
1. **Gradient Boosting Classifier** emerged as the top-performing model with **97.4% accuracy**, demonstrating its effectiveness in detecting suspicious URLs.
2. Features like **HTTPS presence**, **anchor tags**, and **website traffic data** were critical for classification.
3. This project provided hands-on experience with data preprocessing, feature engineering, and model optimization.

---

## Future Enhancements 🔮
- **Real-Time Detection**: Integrate with browser extensions or APIs for real-time URL detection.
- **Enhanced Features**: Utilize advanced NLP techniques to extract semantic features from URLs.
- **Threat Analysis**: Extend the system to detect malicious attachments and embedded threats.

---

## Contributing 🤝
We welcome contributions to improve the project! Feel free to open issues, submit pull requests, or suggest new features.

---

## License 📜
This project is licensed under the **MIT License**. Feel free to use and modify the code.

---

## Acknowledgments 🙏
Special thanks to all contributors and the open-source community for their support.

---

Happy Coding! 🚀
