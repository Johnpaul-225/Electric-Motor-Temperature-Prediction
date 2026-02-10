# Electric Motor Temperature Prediction using Machine Learning

## 📌 Project Overview
Electric motors are widely used in industrial applications, and overheating can lead to performance degradation, equipment failure, and increased maintenance cost.  
This project uses **Machine Learning techniques** to predict the **rotor temperature of an electric motor** based on historical sensor data such as voltage, current, motor speed, and stator temperatures.

The trained model is deployed using a **Flask web application** that allows users to predict motor temperature through a manual input interface and demonstrates a future-ready sensor-based prediction module.

---

## 🎯 Objectives
- Identify the problem as a **regression task**
- Perform **data analysis and preprocessing**
- Train and compare multiple **machine learning regression models**
- Select the best-performing model based on **RMSE and R² score**
- Deploy the model using a **Flask web application**
- Demonstrate predictive maintenance use cases

---

## 🧠 Machine Learning Models Used
- Linear Regression  
- Decision Tree Regressor ✅ (Final Model)
- Random Forest Regressor (optional comparison)
- Support Vector Regressor (conceptual comparison)

**Best Model:** Decision Tree Regressor  
**Performance:**  
- R² Score ≈ 96%  
- Low RMSE  

---

## 🛠️ Technology Stack
- **Python 3.9**
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Flask
- HTML, CSS

---

## 📁 Project Structure
Electric-Motor-Temperature-Prediction/
│
├── Dataset/
│ └── measures_v2.csv
│
├── Notebook/
│ ├── Rotor_Temperature_Detection.ipynb
│ ├── model.save
│ └── transform.save
│
├── Flask/
│ ├── app.py
│ ├── model.save
│ ├── transform.save
│ ├── templates/
│ │ ├── home.html
│ │ ├── manual_predict.html
│ │ └── sensor_predict.html
│ └── static/
│ └── style.css
│
├── Report/
│ └── Project_Report.docx
│
└── README.md


---

## 📊 Dataset Description
The dataset consists of real-world motor sensor readings, including:
- Ambient temperature  
- Coolant temperature  
- Voltage (d-axis, q-axis)  
- Current (d-axis, q-axis)  
- Motor speed  
- Stator yoke temperature  
- Stator winding temperature  
- Rotor temperature (target variable)

---

## ⚙️ How to Run the Project
🔹 Step 1: Install Dependencies
pip install numpy pandas matplotlib seaborn scikit-learn flask

🔹 Step 2: Train the Model
Open Notebook/Rotor_Temperature_Detection.ipynb

Select Python 3.9 kernel

Run all cells from top to bottom

Ensure model.save and transform.save are generated

🔹 Step 3: Copy Model Files
Copy:

Notebook/model.save
Notebook/transform.save
Paste into:

Flask/
🔹 Step 4: Run Flask Application
cd Flask
python app.py
Open browser and visit:

http://127.0.0.1:5000
🖥️ Application Features
1️⃣ Manual Prediction
User manually enters motor parameters

Model predicts rotor temperature instantly

Used for demo and testing

2️⃣ Sensor-Based Prediction
Conceptual module for real-time IoT integration

Demonstrates future scope of the system

🧪 Sample Manual Input (For Demo)
Ambient Temperature: 25

Coolant Temperature: 30

Voltage d-axis: 0.5

Voltage q-axis: 1.2

Motor Speed: 1200

Current d-axis: -1

Current q-axis: 5

Stator Yoke Temperature: 45

Stator Winding Temperature: 60

🧩 Use Cases
Predictive maintenance

Overheating prevention

Energy efficiency optimization

Equipment reliability improvement

🚀 Future Enhancements
Real-time IoT sensor integration

Cloud deployment

Deep learning models

Mobile and dashboard-based monitoring

🎓 Academic Note
This project is developed for educational and academic purposes and demonstrates the practical application of machine learning in predictive maintenance systems.

📜 License
This project is open for academic use and learning purposes.


---


