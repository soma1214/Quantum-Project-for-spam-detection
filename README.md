📌 Spam Detection Using Classical & Quantum Naive Bayes

A comparative study of Classical Naive Bayes, Quantum Naive Bayes, and Advanced Quantum Naive Bayes for SMS spam detection, along with a fully functional Spam Detector Web App built using Gradio.

👥 Team Members
Name	Roll Number
Soma Shekar Reddy	22BDS022
Aravind	22BDS015
Stephen	22BEC050
Mahidar	22BEC022
Sriram Bhargav	22BEC029
📖 Project Overview

Spam messages pose a growing threat on SMS, email, and communication platforms.
Traditional machine learning methods like Naive Bayes are effective for spam detection, while Quantum Machine Learning (QML) is an emerging field aimed at achieving better performance using quantum computation.

This project implements and compares:

✔ Classical Naive Bayes
✔ Quantum Naive Bayes
✔ Advanced Quantum Naive Bayes

A Gradio-based web application allows users to classify any message as SPAM or HAM using any of the above models.

🔧 Technologies Used
Languages & Libraries

Python

Qiskit

Pennylane

Scikit-Learn

Pandas & NumPy

Matplotlib

Gradio (App UI)

Quantum Frameworks

Qiskit (default.qubit simulator)

Pennylane (Quantum Nodes / Hybrid models)

📊 Dataset

Using the SMS Spam Collection Dataset (UCI):

Label	Count
Ham	966
Spam	149
Total	1115

Preprocessing steps include:

Lowercasing

Stopword removal

CountVectorizer with top 1000 features

80:20 train-test split

🤖 Models Implemented
1️⃣ Classical Naive Bayes

MultinomialNB

Best performance on text

Baseline model

2️⃣ Quantum Naive Bayes

4-qubit circuit

AmplitudeEmbedding

Rotational layers + CNOT entanglement

Hybrid probability mixing (70% classical, 30% quantum)

3️⃣ Advanced Quantum Naive Bayes

3-qubit circuit

RY/RZ variational layers

CZ entanglement

Extracted quantum feature → GaussianNB

Experimental hybrid QML model

🧪 Results
📌 Classical Naive Bayes

➡ Accuracy: 98.39%
Excellent spam/ham separation.

📌 Quantum Naive Bayes

➡ Accuracy: 89.69%
Strong ham detection but weak spam recall.

📌 Advanced Quantum NB

➡ Accuracy: 15.00%
Highly unstable due to extreme feature compression.

📉 Accuracy Comparison

Model	Accuracy
Classical NB	0.9839
Quantum NB	0.8969
Advanced QNB	0.1500
🖥️ Spam Detector Web App
The app allows real-time message testing with 3 models:

✔ Classical
✔ Quantum
✔ Advanced Quantum

Example UI:
Message:  Win $1000 now! Click here!
Model:    Classical
Result:   SPAM


Screenshots available in /images/.

🚀 How to Run the Project
1. Install Required Libraries
pip install qiskit qiskit-machine-learning qiskit-algorithms pandas scikit-learn qiskit-aer pennylane gradio

2. Run the Jupyter Notebook
jupyter notebook quantum_ai.ipynb

3. Start the Spam Detector App
python simple_spam_app.py


The app will open in your browser locally.

🧠 Key Findings

Classical Naive Bayes still performs best for NLP tasks.

Quantum models struggle with:

High dimensional data

Feature compression

Limited qubits

QML is promising but not yet ready for real-world text applications.

🔮 Future Enhancements

Implement Quantum SVM or Quantum Neural Networks

Use angle or flexible feature embedding

Increase dataset size

Deploy app online

Test using real IBM Quantum hardware

📚 References

Qiskit Documentation

Pennylane Documentation

Scikit-learn Docs

SMS Spam Collection Dataset (UCI ML Repository)

Research papers on Quantum Machine Learning
