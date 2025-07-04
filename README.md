# 🧠 Multiple Disease Prediction Web App

A **multi-disease prediction system** built using **Streamlit** and **Machine Learning models** to detect:
* 🩸 **Diabetes**
* ❤️ **Heart Disease**
* 🧠 **Parkinson's Disease**

🔗 **Live App**: https://multiple-disease-prediction-test-therealvinayak.streamlit.app/

## 🚀 Features

* 🧪 Predict the likelihood of **three major diseases** based on health parameters
* 💡 Powered by trained **ML classification models**
* 📊 Clean, interactive **Streamlit UI**
* 📱 Mobile-friendly and responsive layout
* ⚡ Real-time predictions with instant results
* 🎯 High accuracy models trained on validated datasets

## 📦 Tech Stack

* **Frontend/UI**: Streamlit
* **Backend**: Scikit-learn, Pandas, NumPy
* **Deployment**: Streamlit Cloud
* **ML Models**: Logistic Regression, SVM, Random Forest (per disease)
* **Data Processing**: Pandas, NumPy
* **Model Serialization**: Pickle

## 🖥️ App Screenshots

![image](https://github.com/user-attachments/assets/d0d68689-ee13-4159-8098-69955abc3b94)
![image](https://github.com/user-attachments/assets/0d4217c0-4b87-49bd-be75-50bd5e4f7d86)
![image](https://github.com/user-attachments/assets/b1d67935-4cb1-40db-b318-9603769d26e7)


## 🛠️ Installation (Local)

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup Instructions

1. **Clone the repository**
```bash
git clone https://github.com/therealvinayak/multiple-disease-prediction.git
cd multiple-disease-prediction
```

2. **Create virtual environment** (recommended)
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run the app**
```bash
streamlit run app.py
```

5. **Access the app**
   - Open your browser and go to `http://localhost:8501`

## 📝 Usage

1. **Select Disease Type**: Choose from Diabetes, Heart Disease, or Parkinson's Disease using the sidebar
2. **Input Health Parameters**: Enter the required health metrics and symptoms
3. **Get Prediction**: Click the predict button to get instant results
4. **View Results**: See the prediction probability and risk assessment

### Input Parameters by Disease:

**Diabetes Prediction:**
- Glucose level, Blood pressure, BMI, Age, etc.

**Heart Disease Prediction:**
- Chest pain type, Cholesterol, Maximum heart rate, etc.

**Parkinson's Disease Prediction:**
- Voice measurements, Tremor indicators, Motor symptoms, etc.

## ⚙️ Deployment

### Streamlit Cloud Deployment

1. **Push to GitHub**: Ensure your code is pushed to a GitHub repository
2. **Connect to Streamlit Cloud**: 
   - Go to [streamlit.io/cloud](https://streamlit.io/cloud)
   - Connect your GitHub account
   - Select your repository
3. **Configure Deployment**:
   - Set `app.py` as the main entry point
   - Add any required secrets/environment variables
4. **Deploy**: Click deploy and your app will be live!

### Local Deployment with Docker (Optional)

```bash
# Build Docker image
docker build -t disease-prediction-app .

# Run container
docker run -p 8501:8501 disease-prediction-app
```

## 📁 Project Structure

```
multiple-disease-prediction/
├── app.py                      # Main Streamlit application
├── models/                     # Trained ML models
│   ├── diabetes_model.pkl
│   ├── heart_disease_model.pkl
│   └── parkinsons_model.pkl
├── data/                       # Dataset files (if included)
├── notebooks/                  # Jupyter notebooks for model training
├── utils/                      # Utility functions
├── requirements.txt            # Python dependencies
├── .streamlit/
│   ├── config.toml            # Streamlit configuration
│   └── secrets.toml           # Secret keys (not in repo)
├── screenshots/               # App screenshots
├── Dockerfile                 # Docker configuration (optional)
├── .gitignore                 # Git ignore file
├── LICENSE                    # License file
└── README.md                  # This file
```

## 🧠 Models & Data

### Machine Learning Models
- **Diabetes Model**: Trained on Pima Indian Diabetes Dataset
- **Heart Disease Model**: Trained on Cleveland Heart Disease Dataset  
- **Parkinson's Model**: Trained on UCI Parkinson's Dataset

### Model Performance
| Disease | Algorithm | Accuracy | Precision | Recall | F1-Score |
|---------|-----------|----------|-----------|--------|----------|
| Diabetes | Logistic Regression | 85% | 0.83 | 0.87 | 0.85 |
| Heart Disease | Random Forest | 88% | 0.86 | 0.89 | 0.87 |
| Parkinson's | SVM | 92% | 0.91 | 0.93 | 0.92 |

### Data Sources
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- Publicly available medical datasets

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Areas for Contribution:
- Adding new disease prediction models
- Improving model accuracy
- Enhancing UI/UX
- Adding data visualizations
- Writing tests
- Improving documentation

## 📊 Future Enhancements

- [ ] Add more disease prediction models
- [ ] Implement deep learning models
- [ ] Add data visualization charts
- [ ] Create REST API endpoints
- [ ] Add user authentication
- [ ] Implement prediction history
- [ ] Add model explainability features
- [ ] Mobile app version

## ⚠️ Disclaimer

This application is for educational and informational purposes only. It should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult with qualified healthcare professionals for medical concerns.

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## ✍️ Author

**Vinayak**
- GitHub: [@therealvinayak](https://github.com/therealvinayak)
- 
## 🙏 Acknowledgments

- UCI Machine Learning Repository for datasets
- Streamlit team for the amazing framework
- Scikit-learn contributors
- Open source community

---

⭐ **If you found this project helpful, please consider giving it a star!** ⭐
