# 🏥 Insurance Cost Prediction using Linear Regression

This project uses **Linear Regression** to predict health insurance costs based on user inputs such as age, BMI, number of children, and smoking status. It utilizes the **Medical Insurance Dataset** and converts the final prediction to **INR (₹)**.

---

## 📊 Dataset

The dataset used is `insurance.csv` containing:

- `age`: Age of the primary beneficiary
- `sex`: Gender of the beneficiary
- `bmi`: Body mass index
- `children`: Number of children/dependents covered by insurance
- `smoker`: Whether the person is a smoker (`yes` or `no`)
- `region`: Residential area in the US
- `charges`: Individual medical costs billed by health insurance (target variable)

---

## 🧠 Features Used

After preprocessing, the model uses the following features:

- `age`
- `bmi`
- `children`
- `smoker` (encoded as 1 for "yes" and 0 for "no")

**Note**: `sex` and `region` are removed as they are not used in model training.

---

## ⚙️ How to Run

1. Make sure you have Python installed (version 3.6+ recommended).
2. Install required libraries:
   ```bash
   pip install pandas scikit-learn
Clone this repository and place your dataset in the correct folder:
dataset/insurance.csv
Run the script:
python insurance_prediction.py
Enter the user details when prompted:
Age
BMI
Number of children
Smoker status (yes/no)
Region (ignored in prediction, for UI purpose)
Gender (ignored in prediction, for UI purpose)
🧮 Model Performance

The model splits the data into 80% training and 20% testing and calculates:
Train Score (R²)
Test Score (R²)
RMSE (Root Mean Squared Error)
💰 Output

The model predicts the insurance cost in USD, which is then converted to INR using an approximate rate of 1 USD = ₹83.
Predicted Insurance Cost: ₹41250.65
📂 File Structure

insurance-prediction/
│
├── dataset/
│   └── insurance.csv
│
├── insurance_prediction.py
└── README.md
📌 Future Improvements

Add more feature engineering
Improve model performance with advanced algorithms (RandomForest, XGBoost)
Build a web UI using Flask or Streamlit for user interaction
👨‍💻 Author

Daniel Christopher M
📄 License

This project is licensed under the MIT License.
