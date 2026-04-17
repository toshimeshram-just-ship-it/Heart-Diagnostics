HeartGuard AI: Integrated Cardiac Diagnostic System
Industry Capstone Project - Track B (Solution Architecture)
📌 Project Overview
HeartGuard AI is an end-to-end clinical decision support system designed to bridge the gap between raw patient data and actionable medical insights. In high-pressure environments like the ICU or ER, medical staff often suffer from "Alert Fatigue." This project provides a hybrid solution that combines Deep Learning (Neural Networks) with Traditional Clinical Rules to prioritize high-risk patients accurately.

🚀 Business Value & "The Why"
Precision Triage: Moves beyond simple "out-of-range" beeps to AI-driven probability scores.

Operational Efficiency: Automates the initial diagnostic scan, allowing doctors to focus on "red-flag" cases first.

Safety First: Uses a hybrid logic gate—if the AI is unsure but vitals are critical (e.g., Tachycardia), the system triggers an immediate manual review.

🛠️ Technical Stack
Language: Python 3.x

Deep Learning: TensorFlow / Keras (Multi-Layer Perceptron)

Data Science: Pandas, NumPy, Scikit-Learn

Visualization: Matplotlib, Seaborn

Environment: Google Colab / Jupyter Notebooks

🧠 System Architecture
The system is built on a Modular Pipeline Architecture, ensuring the AI model is decoupled from the clinical business logic.

Synthetic Data Engine: Generates industry-grade medical records (5,000+ samples) including Age, BMI, Cholesterol, Systolic BP, and Lifestyle factors.

Neural Network (MLP): A 4-layer deep architecture with Dropout Regularization (20%) to prevent overfitting and ensure real-world generalizability.

Hybrid Inference Layer: A custom diagnostic loop that maps AI risk scores to specific patient identities and triggers alerts based on both neural predictions and clinical thresholds (e.g., Hypertension detection).

📊 Key Results & Failure Analysis
Accuracy: Achieved high precision/recall on synthetic test sets.

Model Validation: Utilized Confusion Matrices to analyze False Negatives (the most dangerous errors in medicine).

Mitigation: Implemented a conservative classification threshold (>0.4 risk) to ensure maximum patient safety.

📁 Repository Structure
Plaintext
├── HeartGuard_AI.ipynb        # Main Capstone Notebook (Code & Report)
├── heart_data_large.csv       # Synthesized Industry Dataset
├── README.md                  # Project Documentation
└── (Optional) requirements.txt # Environment dependencies
💻 How to Run
Open the .ipynb file in Google Colab or a local Jupyter environment.

Run the Data Generation cell to create the heart_data_large.csv.

Execute the Training cells to build the MLP model.

Run the Clinical Report section to see the real-time patient diagnostic dashboard in action.

🔮 Future Roadmap
IoT Integration: Connecting to wearable sensors (Apple Watch/Fitbit) for 24/7 live monitoring.

Multi-Modal AI: Incorporating X-ray image analysis to create a 360-degree patient health view.

Federated Learning: Training models across multiple hospital databases while maintaining strict patient privacy.

Author: Toshi Meshram
